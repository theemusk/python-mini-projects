def calculate_grade(percentage):
    if percentage >= 90:
        return "A+"
    elif percentage >= 80:
        return "A"
    elif percentage >= 70:
        return "B"
    elif percentage >= 60:
        return "C"
    elif percentage >= 40:
        return "D"
    else:
        return "F"


def main():
    print("=== Student Grade Calculator ===")

    try:
        count = int(input("Number of subjects: "))

        if count <= 0:
            print("Enter a positive number of subjects.")
            return

        marks = []

        for i in range(count):
            mark = float(input(f"Marks in subject {i + 1} (0-100): "))

            if not 0 <= mark <= 100:
                print("Marks must be between 0 and 100.")
                return

            marks.append(mark)

        total = sum(marks)
        percentage = total / count

        print(f"\nTotal marks: {total:g}/{count * 100}")
        print(f"Percentage: {percentage:.2f}%")
        print(f"Grade: {calculate_grade(percentage)}")

    except ValueError:
        print("Please enter valid numbers.")


if __name__ == "__main__":
    main()
