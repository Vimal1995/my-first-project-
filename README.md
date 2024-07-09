# my-first-project-
survival duration calculator
def calculate_duration(age, time_unit):
    conversion_factors = {
        'months': 12,
        'weeks': 52,
        'days': 365,
        'hours': 365 * 24,
        'minutes': 365 * 24 * 60,
        'seconds': 365 * 24 * 60 * 60
    }
    duration = age * conversion_factors.get(time_unit.lower(), 1)
    return duration
age = int(input("What's your age? "))
time_unit = input("Please choose time unit: Months, Weeks, Days, Hours, Minutes, Seconds. ")
duration = calculate_duration(age, time_unit)
print(f"You lived for {duration} {time_unit}.")
