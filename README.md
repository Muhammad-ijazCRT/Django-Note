# Django-Note
Django Note



### Read csv file in django
https://studygyaan.com/django/how-to-export-csv-file-with-django

    import csv 
    def index(request):
    with open("email.csv", "r") as csvfile:
        reader = csv.reader(csvfile)
        for row in reader:
            print(row)
    return render(request, 'polls/index.html')


###

### “how to iterate multiple array in django template” Code Answer’s

    mylist = zip(list1, list2)
    context = {
                'mylist': mylist,
            }
    return render(request, 'template.html', context)
    
##### loop for 
    {% for item1, item2 in mylist %}
