# bungacans
------------------------ PROFIL---------------------
import 'package:flutter/material.dart';

class Login extends StatefulWidget {
  Login({Key key}) : super(key: key);

  @override
  _LoginState createState() => _LoginState();
}

class _LoginState extends State<Login> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: PreferredSize(
        preferredSize: Size.fromHeight(0),
        child: AppBar(),
      ),
      body: SingleChildScrollView(
        child: Padding(
          padding: const EdgeInsets.all(20),
          child: Column(
            crossAxisAlignment: CrossAxisAlignment.start,
            children: [
              Container(
                padding: EdgeInsets.only(top: 0, bottom: 0, left: 10, right: 0),
                child: Text(
                  'Bunga Anggi Safitri',
                  style: TextStyle(
                    fontSize: 20,
                    fontWeight: FontWeight.bold,
                  ),
                ),
              ),
              new Image.asset(
                "img/bunga.jpeg",
                width: 200.0,
              ),
              Container(
                padding: EdgeInsets.only(top: 0, bottom: 0, left: 10, right: 0),
                child: Text(
                  'NO HP : 0815-1739-0140',
                  style: TextStyle(
                    fontSize: 20,
                    fontWeight: FontWeight.bold,
                  ),
                ),
              ),
              Container(
                padding: EdgeInsets.only(top: 0, bottom: 0, left: 10, right: 0),
                child: Text(
                  'EMAIL :  bungaanggisafitri@gmail.com',
                  style: TextStyle(
                    fontSize: 20,
                    fontWeight: FontWeight.bold,
                  ),
                ),
              ),
              const SizedBox(
                height: 20,
              ),
              Container(
                padding: EdgeInsets.only(top: 0, bottom: 0, left: 10, right: 0),
                child: Text(
                  'Ku wakili bersyukur dari ratusan hari yang lalu di hari ini. Segala luka, segala kecewa dan kegagalan kutinggalkan di hari yang lalu. Berjuta syukur dengan segala cobaan dan ujian. Aku masih bernafas dan aku baik² saja. Semoga selalu dalam lindungan, Ridho dan kuasa ny .. Aamiin -Bungaasftr❤',
                  style: TextStyle(
                    fontSize: 20,
                    fontWeight: FontWeight.bold,
                  ),
                ),
              ),
              Card(
                color: Colors.black87,
                elevation: 10,
                child: Container(
                  height: 50,
                  child: InkWell(
                    splashColor: Colors.white,
                    onTap: () {},
                    child: Center(
                      child: Text(
                        "EDIT",
                        style: TextStyle(fontSize: 20, color: Colors.white),
                      ),
                    ),
                  ),
                ),
              )
            ],
          ),
        ),
      ),
    );
  }
}

-------------------------------------- end----------------------
------------------------------------- Login---------------
import 'package:flutter/material.dart';

class Login extends StatefulWidget {
  Login({Key key}) : super(key: key);

  @override
  _LoginState createState() => _LoginState();
}

class _LoginState extends State<Login> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Container(
        width: MediaQuery.of(context).size.width,
        padding: const EdgeInsets.all(8),
        color: Colors.lightBlue,
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            Container(
              width: 100,
              height: 100,
              decoration:
                  BoxDecoration(color: Colors.black87, shape: BoxShape.circle),
              child: Center(
                child: Icon(
                  Icons.person,
                  size: 40,
                  color: Colors.white,
                ),
              ),
            ),
            SizedBox(
              height: 20,
            ),
            Text(
              "Selamat DATANG Silahkan Login",
              style: TextStyle(fontSize: 20, color: Colors.black87),
            ),
            SizedBox(
              height: 20,
            ),
            TextFormField(
              decoration: InputDecoration(
                border: OutlineInputBorder(),
                focusedBorder: OutlineInputBorder(
                    borderSide: BorderSide(color: Colors.black87)),
                prefixIcon: Icon(
                  Icons.person,
                  size: 40,
                ),
                hintText: "Masukkan Username",
                hintStyle: TextStyle(color: Colors.black87),
                labelText: "Username",
                labelStyle: TextStyle(color: Colors.black87),
              ),
            ),
            SizedBox(
              height: 20,
            ),
            TextFormField(
              obscureText: true,
              decoration: InputDecoration(
                border: OutlineInputBorder(),
                focusedBorder: OutlineInputBorder(
                    borderSide: BorderSide(color: Colors.black87)),
                prefixIcon: Icon(
                  Icons.lock,
                  size: 40,
                ),
                hintText: "Masukkan Password",
                hintStyle: TextStyle(color: Colors.black87),
                labelText: "Password",
                labelStyle: TextStyle(color: Colors.black87),
              ),
            ),
            SizedBox(
              height: 20,
            ),
            Card(
              color: Colors.black87,
              elevation: 5,
              child: Container(
                height: 50,
                child: InkWell(
                  splashColor: Colors.white,
                  onTap: () {},
                  child: Center(
                    child: Text(
                      "Masuk",
                      style: TextStyle(fontSize: 20, color: Colors.white),
                    ),
                  ),
                ),
              ),
            )
          ],
        ),
      ),
    );
  }
}

