# Calculator-
def display_input(input_str):
    print("You entered:", input_str)

def main():
    input_str = ""
    while True:
        key = input("Press a key: ")
        if key == "":
            continue
        if key in ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]:
            input_str += key
            print("Appended key to input:", input_str)
        elif key == "#":
            display_input(input_str)
            input_str = ""
        elif key == "*":
            break
        else:
            print("Invalid key:", key)
            input_str = ""

if __name__ == "__main__":
    main()
