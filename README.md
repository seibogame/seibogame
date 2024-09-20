def juego_seibo():
    print("¡Bienvenido al juego de Verdadero y Falso sobre el Seibo!")
    print("Responde 'V' para Verdadero y 'F' para Falso.\n")

    preguntas = [
        {
            "texto": "El seibo es un árbol nativo de América tropical.",
            "respuesta": "V"
        },
        {
            "texto": "El seibo puede crecer hasta 30 metros de altura.",
            "respuesta": "V"
        },
        {
            "texto": "Las flores del seibo son de color azul.",
            "respuesta": "F"
        },
        {
            "texto": "El seibo es considerado un árbol sagrado en algunas culturas.",
            "respuesta": "V"
        },
        {
            "texto": "El fruto del seibo no se utiliza en la industria textil.",
            "respuesta": "F"
        }
    ]

    puntuacion = 0

    for pregunta in preguntas:
        print(pregunta["texto"])
        respuesta_usuario = input("Tu respuesta (V/F): ").strip().upper()
        
        if respuesta_usuario == pregunta["respuesta"]:
            print("¡Correcto!\n")
            puntuacion += 1
        else:
            print("Incorrecto. La respuesta correcta es:", "V" if pregunta["respuesta"] == "V" else "F", "\n")

    print(f"Tu puntuación final es: {puntuacion}/{len(preguntas)}")
    
juego_seibo()
