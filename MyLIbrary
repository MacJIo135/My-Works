class MyLibrary:
    flag = True
    books = []

    while flag:
        print(' 1: Add book to the library\n 2: Delete book from library\n 3: Search book\n 4: Show list books\n 5: Show discription')
        action = int(input())
        if action == 1:
            amount = int(input('Please, input quantity of book = '))
            for i in range(amount):
                n = 0
                print('Please, write Title book, Author, Edition and Year of edition of the book separated by a comma(For example: Forest, Lesya, Gold Edition, 1987):')
                value = [i for i in input().split(', ')]
                print('Enter discription of book:')
                key = input()
                dicts = {key: value}
                books.append(dicts)
        elif action == 2:
            if len(books) == 0:
                print('You dont have books in library')
            else:
                print('Please, write number of book, which you want to delete or press 0 to back menu:')
                n = 1
                for i in books:
                    for j in i.values():

                        print(n, ': ', *j)
                n = n + 1
                number = int(input())
                number -= 1
                if number == 0:
                    print('You have exited to the previous menu')
                else:
                    del books[number]
        elif action == 3:
            if len(books) == 0:
                print('')
            else:
                print('''Please, input Title of book, Author, Edition and Year of Edition of the book separated by comma(For example: Forest, Lesya, Gold Edition, 1987):''')
                search = [i for i in input().split(', ')]
                for i in books:
                    for key, value in i.items():
                        sum = 0
                        if search == value:
                            sum += 1
                    if sum == 1:
                        print('This book was found')
                        break
                    else:
                        print('This book not found')
                        break
        elif action == 4:
            if len(books) == 0:
                print('You dont have books in library')
            else:
                n = 1
                for i in books:
                    for j in i.values():
                        print(n, ': ', *j)
                    n = n + 1
        elif action == 5:
            if len(books) == 0:
                print('You dont have books in the library')
            else:
                print('Enter number of book which you want read discription:')
                n = 1
                for i in books:
                    for j in i.values():
                        print(n, ': ', *j)
                    n = n + 1
                number = int(input())
                number -= 1
                print(*books[number])
