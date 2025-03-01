# This is a list of days in a week
days_in_a_week = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']

# This is a list tracking hours of sleep every day
sleep_hours = []


# This is a function that gets hours of sleep of one night from the user
def get_hours_of_sleep(day):
    while True:
        daily_sleep_hour = float(input('How many hours did you sleep on ' + day + ' night? '))
        if daily_sleep_hour < 0 or daily_sleep_hour > 24:
            print('Invalid input. Please enter a number between 0 and 24.')
            continue
        else:
            break
    return daily_sleep_hour


# This is a function that calculate the average sleep hour of a week
def calculate_average_sleep_hour(list_of_hours):
    average_sleep_hour = sum(list_of_hours) / len(list_of_hours)
    return average_sleep_hour


# This is the main function that calls the other two functions and identify your sleeping pattern of the week
def main():
    for day in days_in_a_week:
        sleep_hours.append(get_hours_of_sleep(day))
    average_sleep = calculate_average_sleep_hour(sleep_hours)
    print(('Your average daily hours of sleep this week is ' + str(average_sleep)) + ' hours')
    if average_sleep >= 7:
        print('You have enough sleep.')
    else:
        print('You need more sleep.')


print('Welcome to the Sleep Hour Calculator!')
while True:
    main()
    keep_going = input('Calculate again? yes / no: ')
    if keep_going == 'yes':
        continue
    else:
        print('Goodbye')
        break
