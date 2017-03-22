#lang racket

(define selection_sort
  (lambda (source dest dis)
    (cond ((and   (empty? source) (empty? dis)) dest)
          ((empty? dest) (selection_sort (cdr source) (cons (car source) dest) dis))
          ((empty? source) (selection_sort (cdr dis) (cons (car dis) dest) source))
          ((< (car dest) (car source)) (selection_sort (cdr source) (cons (car source) (cdr dest)) (cons (car dest) dis)))
          (else (selection_sort (cdr source) dest (cons (car source) dis))))))


(selection_sort '(1 5 8 3 1 7 5 9) '() '())