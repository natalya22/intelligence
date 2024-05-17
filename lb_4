(deftemplate book
    (slot title)
    (slot author)
    (slot genre)
    (slot time_period)
    (slot country)
)

(deffacts books
    (book (title "Pride and Prejudice") (author "Jane Austen") (genre "Romance") (time_period "Regency") (country "England"))
	(book (title "Pride and Prejudice") (author "Jane Austen") (genre "e") (time_period "e") (country "e"))
    (book (title "1984") (author "George Orwell") (genre "Dystopian") (time_period "Future") (country "N/A"))
    (book (title "The Great Gatsby") (author "F. Scott Fitzgerald") (genre "Classic") (time_period "1920s") (country "USA"))
    (book (title "To Kill a Mockingbird") (author "Harper Lee") (genre "Drama") (time_period "1930s") (country "USA"))
    (book (title "One Hundred Years of Solitude") (author "Gabriel Garcia Marquez") (genre "Magical Realism") (time_period "20th Century") (country "Colombia"))
)

(defrule start
    (declare (salience 10))
    =>
    (printout t "Welcome to the Book Recommendation System!" crlf)
    (printout t "Please answer the following questions to receive book recommendations." crlf)
    (printout t crlf)
)

(defrule ask_genre
    (not (genre ?))
    =>
    (printout t "What genre are you interested in? (Romance, Dystopian, Classic, Drama, Magical Realism): ")
    (assert (genre (read)))
)

(defrule ask_time_period
    (not (time_period ?))
    =>
    (printout t "In what time period would you like to find yourself? (Regency, Future, 1920s, 1930s, 20th Century): ")
    (assert (time_period (read)))
)

(defrule ask_country
    (not (country ?))
    =>
    (printout t "In which country would you like to immerse yourself? (England, USA, Colombia): ")
    (assert (country (read)))
)

(defrule recommend_books

(genre ?genre)
(time_period ?time_period)
(country ?country)

;(book (title ?title) (author ?author) (genre ?genre) (time_period ?time_period) (country ?country))
=>
;(printout t "Title: " ?title crlf)
(printout t "Author: " ?author crlf)
(printout t "Genre: " ?genre crlf)
(printout t "Time Period: " ?time_period crlf)
(printout t "Country: " ?country crlf)
;(printout t crlf)
)
