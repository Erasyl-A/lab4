
from datetime import datetime, timedelta

def subtract_five_days():
    return datetime.now() - timedelta(days=5)

def print_dates():
    today = datetime.now()
    yesterday = today - timedelta(days=1)
    tomorrow = today + timedelta(days=1)
    return yesterday, today, tomorrow

def drop_microseconds():
    return datetime.now().replace(microsecond=0)

def date_difference_in_seconds(date1, date2):
    delta = date2 - date1
    return delta.total_seconds()

if __name__ == "__main__":
    print("Date 5 days ago:", subtract_five_days())
    y, t, tm = print_dates()
    print("Yesterday:", y)
    print("Today:", t)
    print("Tomorrow:", tm)
    print("Datetime without microseconds:", drop_microseconds())
    print("Difference in seconds:", date_difference_in_seconds(datetime(2024, 2, 10), datetime(2024, 2, 16)))
