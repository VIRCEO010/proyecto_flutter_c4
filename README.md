# proyecto_flutter_c4
vinil plus

main.dart
import 'package:flutter/material.dart';
import 'pages/registrovinilos.dart';

import 'pages/login.dart';

void main(List<String> args) {
  runApp(
    const MaterialApp(
      title: "Mi primera aplicacion",
      home: RegistroPage(),
    ),
  );
}


login.dart

import 'package:flutter/material.dart';

class LoginPage extends StatelessWidget {
  const LoginPage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Color.fromARGB(255, 63, 200, 226),
      body: SingleChildScrollView(
        child: Padding(
          padding: const EdgeInsets.all(20),
          child: Column(
            children: [
              const SizedBox(
                height: 20,
              ),
              Image.asset("assets/images/vinilplus(2)sinfondo(1).png"),
              const SizedBox(
                height: 5,
              ),
              const TextField(
                obscureText: true,
                decoration: InputDecoration(
                  border: OutlineInputBorder(),
                  labelText: 'Email addres',
                ),
              ),
              const SizedBox(
                height: 10,
              ),
              const TextField(
                obscureText: true,
                decoration: InputDecoration(
                  border: OutlineInputBorder(),
                  labelText: 'Paswword',
                ),
              ),
              const SizedBox(
                height: 10,
              ),
              ElevatedButton(
                child: const Text("Iniciar Sesion"),
                onPressed: () {},
              ),
              const SizedBox(
                height: 10,
              ),
              const Text("O iniciar sesion con:"),
              Row(
                mainAxisAlignment: MainAxisAlignment.spaceEvenly,
                children: [
                  ElevatedButton(
                    child: const Text("Facebook"),
                    onPressed: () {},
                  ),
                  ElevatedButton(
                    child: const Text("Google"),
                    onPressed: () {},
                  ),
                ],
              ),
              const SizedBox(
                height: 5,
              ),
              const Text("no tienes una cuenta?"),
              ElevatedButton(
                child: const Text("Registrate"),
                onPressed: () {},
              )
            ],
          ),
        ),
      ),
    );
  }
}


registrovinilos.dart
import 'package:flutter/material.dart';

class RegistroPage extends StatelessWidget {
  const RegistroPage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Color.fromARGB(255, 63, 200, 226),
      body: SingleChildScrollView(
        child: Padding(
          padding: const EdgeInsets.all(20),
          child: Column(children: [
            const SizedBox(
              height: 20,
            ),
            Image.asset("assets/images/registravinilos.png"),
            const SizedBox(
              height: 10,
            ),
            const SizedBox(
              height: 10,
            ),
            const Text(
              "cuantos vinilos vas a vender",
              style: TextStyle(
                fontSize: 20,
              ),
            ),
            const TextField(
              obscureText: true,
              decoration: InputDecoration(
                border: OutlineInputBorder(),
                labelText: '',
              ),
            ),
            Padding(
              padding: const EdgeInsets.all(20),
            ),
            const SizedBox(
              height: 1,
            ),
            const Text(
              "Genero musical",
              style: TextStyle(
                fontSize: 18,
              ),
            ),
          ]),
        ),
      ),
    );
  }
}


home.dart
import 'package:flutter/material.dart';

class HomePage extends StatelessWidget {
  const HomePage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text("Inicio"),
      ),
      body: const Center(
        child: Text("Hola Mundo"),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: () {},
        child: const Icon(Icons.add),
      ),
    );
  }
}


crearcuenta.dart
import 'package:flutter/material.dart';

class CrearcuentaPage extends StatelessWidget {
  const CrearcuentaPage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Color.fromARGB(255, 63, 200, 226),
      body: SingleChildScrollView(
        child: Padding(
          padding: const EdgeInsets.all(20),
          child: Column(children: [
            const SizedBox(
              height: 20,
            ),
            Image.asset("assets/images/parrafocrearcuentasf.png"),
            const SizedBox(
              height: 10,
            ),
            const TextField(
              obscureText: true,
              decoration: InputDecoration(
                border: OutlineInputBorder(),
                labelText: 'Correo electronico o numero de telefono',
              ),
            ),
            const SizedBox(
              height: 10,
            ),
            const TextField(
              obscureText: true,
              decoration: InputDecoration(
                border: OutlineInputBorder(),
                labelText: 'Nombre completo',
              ),
            ),
            const SizedBox(
              height: 10,
            ),
            const TextField(
              obscureText: true,
              decoration: InputDecoration(
                border: OutlineInputBorder(),
                labelText: 'Nombre de usuario',
              ),
            ),
            const SizedBox(
              height: 10,
            ),
            const TextField(
              obscureText: true,
              decoration: InputDecoration(
                border: OutlineInputBorder(),
                labelText: 'Password',
              ),
            ),
            ElevatedButton(
              child: const Text("Registrate"),
              onPressed: () {},
            ),
            const SizedBox(
              height: 50,
            ),
            const SizedBox(),
            const Text("Tienes una cuenta?"),
            ElevatedButton(
              child: const Text("Inicia sesion"),
              onPressed: () {},
            ),
            const SizedBox(
              height: 50,
            ),
          ]),
        ),
      ),
    );
  }
}
