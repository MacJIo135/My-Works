class MyLibrary:
    def __init__(self):
        self.flag = True
        self.books = []

    def add_book(self):
        self.amount = int(input('Please, input quantity of book = '))
        for i in range(self.amount):
            n = 0
            print('Please, write Title book, Author, Edition and Year of edition of the book separated by a comma(For example: Forest, Lesya, Gold Edition, 1987):')
            value = [i for i in input().split(', ')]
            print('Enter discription of book:')
            key = input()
            dicts = {key: value}
            self.books.append(dicts)

    def delete_book(self):
        if len(self.books) == 0:
            print('You dont have books in library')
        else:
            print('Please, write number of book, which you want to delete or press 0 to back menu:')
            n = 1
            for i in self.books:
                for j in i.values():
                    print(n, ': ', *j)
                n = n + 1
            number = int(input())
            number -= 1
            if number == 0:
                print('You have exited to the previous menu')
            else:
                del self.books[number]

    def serch_book(self):
        if len(self.books) == 0:
            print('You dont have books in library')
        else:
            print('''Please, input Title of book, Author, Edition and Year of Edition of the book separated by comma(For example: Forest, Lesya, Gold Edition, 1987):''')

            search = [i for i in input().split(', ')]

            for i in self.books:
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

    def show_list_books(self):
        if len(self.books) == 0:
            print('You dont have books in library')
        else:
            n = 1
            for i in self.books:
                for j in i.values():
                    print(n, ': ', *j)
                n = n + 1

    def show_discription(self):
        if len(self.books) == 0:
            print('You dont have books in the library')
        else:
            print('Enter number of book which you want read discription:')
            n = 1
            for i in self.books:
                for j in i.values():
                    print(n, ': ', *j)
                n = n + 1
            number = int(input())
            number -= 1
            self.books.sort()
            print(*self.books[number])

    def start_work(self):
        while self.flag:
            print(' 1: Add book to the library\n 2: Delete book from library\n 3: Search book\n 4: Show list books\n 5: Show discription')
            action = int(input())

            if action == 1:
                self.add_book()
            elif action == 2:
                self.delete_book()
            elif action == 3:
                self.serch_book()
            elif action == 4:
                self.show_list_books()
            elif action == 5:
                self.show_discription()


lib1 = MyLibrary()
lib1.start_work()
