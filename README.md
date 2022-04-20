# Django-Note
Django Note


### Read csv file in django

import csv
def index(request):

    with open("email.csv", "r") as csvfile:
        reader = csv.reader(csvfile)
        for row in reader:
            print(row)
    return render(request, 'polls/index.html')
