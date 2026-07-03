def calculate_grade(scores):
    if not scores or len(scores) == 0:
        return "No Data", 0.0 
    average = sum(scores) / len(scores)
    if average >= 80:
        grade = "A"
    elif average >= 70:
        grade = "B"
    elif average >= 60:
        grade = "C"
    elif average >= 50:
        grade = "D"
    else:
        grade = "F"
    return grade, average

