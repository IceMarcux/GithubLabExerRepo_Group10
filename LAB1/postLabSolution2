# Prompt the user for a filename and read in the lines of text into a list
filename = input("Enter the name of the file: ")
with open(filename, 'r') as file:
    lines = file.readlines()

# Enter a loop that prints the number of lines in the file and prompts the user for a line number
while True:
    print("This file has", len(lines), "lines.")
    line_num = input("Enter a line number (0 to quit): ")
    
    # If the user enters 0, quit the program
    if line_num == "0":
        break
    
    # If the user enters a valid line number, print the corresponding line
    try:
        line_num = int(line_num)
        if line_num > 0 and line_num <= len(lines):
            print("Line", line_num, ":", lines[line_num-1])
        else:
            print("Invalid line number. Please enter a number between 1 and", len(lines))
    # If the user enters something that can't be converted to an integer, print an error message
    except ValueError:
        print("Invalid input. Please enter a number.")
