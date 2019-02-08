# Duplicates-Books

def add_book():
    new_book = ui.get_book_info()
    all_books = store.get_all_books()
    if new_book in all_books:
        ui.message('The book already exists')
    else:
        store.add_book(new_book)
        ui.message('New book Added!')
    # TODO show an error message if a book is already in the store, don't add book
