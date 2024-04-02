%Упорядочить список методом пузырька
% Правило для проверки и перестановки элементов в списке
bubble_sort(List, SortedList) :- 
    swap(List, NewList), !, 
    bubble_sort(NewList, SortedList).
bubble_sort(SortedList, SortedList).
% Правило для перестановки двух соседних элементов
swap([X,Y|T], [Y,X|T]) :- 
    X > Y.
swap([Z|T], [Z|NewT]) :- 
    swap(T, NewT).
% Запрос на проверку: bubble_sort([3,1,4,1,5,9,2,6,5], SortedList).
