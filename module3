#1task
from datetime import datetime
def get_days_from_today(date):
    input_date = datetime.strptime(date, '%Y-%m-%d')
    current_date = datetime.today()
    difference = current_date - input_date
    return difference.days

date = '2019-11-05'
print(get_days_from_today(date))


#2task

import random
def get_numbers_ticket(minimum, maximum, quantity):
    if not (1 <= minimum <= maximum <= 1000 and 1 <= quantity <= maximum - minimum + 1):
        return []
    unique_numbers = set()

    while len(unique_numbers) < quantity:
        unique_numbers.add(random.randint(minimum, maximum))

    return sorted(list(unique_numbers))

min_num = 1
max_num = 49
quantity = 6
print(get_numbers_ticket(min_num, max_num, quantity))


#3task

import re

phone_numbers = [
    "    +38(050)123-32-34",
    "     0503451234",
    "(050)8889900",
    "38050-111-22-22",
    "38050 111 22 11 asf  "
]

for phone in phone_numbers:
    # cleaned_number = re.sub(r'\D', '', phone)
    cleaned_number = re.sub(r'[^0-9]', '', phone)
    if not cleaned_number.startswith('+'):
        if cleaned_number.startswith('380'):
            cleaned_number = '+' + cleaned_number
        else:
            cleaned_number = '+38' + cleaned_number
    print(cleaned_number)
