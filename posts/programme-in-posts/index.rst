.. title: Programme in Posts
.. slug: programme-in-posts
.. date: 2016-07-06 18:50:15 UTC+02:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text

Schreibe hier deinen Eintrag hin.

.. code-block:: python
   :number-lines:

   def sieve_of_eratosthenes():
       factors = defaultdict(set)
       for n in count(2):
           if factors[n]:
               for m in factors.pop(n):
                   factors[n+m].add(m)
           else:
               factors[n*n].add(n)
               yield n
