4clojure
========

4Clojure

;; 19. Last Element
;; Write a function which returns the last element in a sequence.
(fn[coll] (nth coll (dec (count coll))))

;; 20. Penultimate Element
;; Write a function which returns the second to last element from
;; a sequence.
#(first (take-last 2 %))

;; 21. Nth Element
;; Write a function which returns the Nth element from a sequence.
#(get (vec %1) %2)

;; 22. Count a Sequence
;; Write a function which returns the total number of elements in a sequence.
#(reduce (fn[x y] (inc x)) 0 %)
