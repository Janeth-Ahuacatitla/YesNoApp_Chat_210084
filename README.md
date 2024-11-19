# yes_no_app


### HISTORIAL DE PRÁCTICAS:

|No.|Nombre|Potenciador|Estatus|
|--|--|--|--|
|22|Implementación de la UI para la Aplicación de Yes/No|10|⭐Activa|
|23|Implementación de la Funcionalidad de la Aplicación de Yes/No|10|⭐Activa|

### OBJETIVO
Facilitar una comunicación rápida, simple y entretenida entre los usuarios mediante mensajes de texto y elementos visuales como GIFs o imágenes. Se busca promover una experiencia más expresiva y cercana, ideal para conversaciones casuales o personales.

### DESCRIPCIÓN
Esta plataforma de mensajería permite a los usuarios comunicarse de manera sencilla y visualmente atractiva. 
De la misma manera permite enviar y recibir texto en tiempo real con un  diseño minimalista y atractivo, con burbujas de diálogo y una interfaz familiar, misma que incluye la opción de finalizar la conversación con un comando específico "?".

### CÓDIGO
import 'package:flutter/material.dart';
import 'package:yes_no_app/domain/entities/message.dart';

class MyMessageBubble extends StatelessWidget {
  final Message message;

  const MyMessageBubble({
    super.key, 
    required this.message
  });

  @override
  Widget build(BuildContext context) {
    final colors = Theme.of(context).colorScheme;

    return Column(
      crossAxisAlignment: CrossAxisAlignment.end,
      children: [
        Container(
          decoration: BoxDecoration(
              color: colors.primary, borderRadius: BorderRadius.circular(20)),
          child: Padding(
            padding: const EdgeInsets.symmetric(horizontal: 20, vertical: 10),
            child: Text(
              message.text,
              style: const TextStyle(color: Colors.white),
            ),
          ),
        ),
        const SizedBox(height: 5)
      ],
    );
  }
}


![Captura de pantalla 2024-11-19 092915](https://github.com/user-attachments/assets/dc602e45-9367-4551-ac63-7df1bdd40e80)
![Captura de pantalla 2024-11-19 093001](https://github.com/user-attachments/assets/081bc688-891d-4a1d-8d42-1d9f530380e6)
![Captura de pantalla 2024-11-19 093144](https://github.com/user-attachments/assets/117d96e8-039f-4ba1-b315-f4f1a6288e59)


### LISTA DE HERRAMIENTAS
![DART](https://img.shields.io/badge/Dart-0175c2?style=for-the-badge&logo=dart&logoColor=white) ![FLUTTER](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)

### AUTOR
Elaborado por: Janeth Ahuacatitla Amixtlan [@Janeth-Ahuacatitla](https://github.com/Janeth-Ahuacatitla)
