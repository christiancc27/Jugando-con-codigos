# Este programa permite al usuario ingresar dos dígitos y luego calcula su suma.

def sum_two_digits():
    """
    Solicita dos dígitos al usuario, los suma y muestra el resultado.
    Maneja errores si la entrada no es un número válido.
    """
    try:
        # Solicitar al usuario el primer dígito
        digit1_str = input("Por favor, ingresa el primer dígito: ")
        # Convertir la entrada a un entero
        digit1 = int(digit1_str)

        # Solicitar al usuario el segundo dígito
        digit2_str = input("Por favor, ingresa el segundo dígito: ")
        # Convertir la entrada a un entero
        digit2 = int(digit2_str)

        # Calcular la suma de los dos dígitos
        suma = digit1 + digit2

        # Mostrar el resultado al usuario
        print(f"La suma de {digit1} y {digit2} es: {suma}")

    except ValueError:
        # Manejar el error si el usuario no ingresa un número válido
        print("Entrada inválida. Por favor, asegúrate de ingresar solo dígitos numéricos.")
    except Exception as e:
        # Manejar cualquier otro error inesperado
        print(f"Ocurrió un error inesperado: {e}")

# Llamar a la función para ejecutar el programa
if __name__ == "__main__":
    sum_two_digits()
