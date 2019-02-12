bad_chars = ["(",")","c","C",".","\\","s","'"]

stripped_test_data = ['1912', '1870-79', '1929',
                      '1913-1923', '1951', '1994', 
                      '1934', '1915', '2009', '1978',
                      '1947', '1995', '1912', '1988',
                      '2002', '1957-1959', '1964-65',
                      '1955', '1970', '1990-1999']

def strip_characters(string):
    for char in bad_chars:
        string = string.replace(char,"")
    string = string.strip()
    return string

def process_date(string):
    if "-" in date:
        split_date = date.split("-")
        date_one = split_date[0]
        date_two = split_date[1]
        if len(date_two) == 2:
            date_two = date_one[:2] + date_two
        date = (int(date_one)+ int(date_two)) / 2
        date = round(date)
    else:
        date = int(date)
    return date

processed_test_data = []

for d in stripped_test_data:
    date = process_date(d)
    processed_test_data.append(data)
    
for row in moma:
    date = row[6]
    date = strip_characters(date)
    date = process_date(date)
    row[6] = date
    
    
