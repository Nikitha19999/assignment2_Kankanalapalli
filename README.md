# assignment2_Kankanalapalli
# Nikitha Srivyshnavi Kankanalapalli
###### Vizag
My favorite place is vizag because of it's long coastal line and it is one of the best places to live in India. I am a huge admirer of nature. I can spend the whole day at the beach. Visakhapatnam has given me the opportunity to live in harmony with nature. From its gushing beaches to the **lush green mountains,the city** has many places to visit with our loved ones to spend some quality time. Vizag, the synonym of beauty {well, at least for us} is one of the best places to live in india and you only realise it once you live here. If you have growth up in some city other than Visakhapatnam, these are the thing you will notice once you come and start living here.

---

# Directions from Marryville to Vizag
1. First I will catch a cab in maryville and travel to kansas City airport. 
2. From Kansas I will catch a flight to chicago.
    1. Next I will catch a flight in Chicago to london
    2. And then there is a 2 hour layover in london
3. Finally my fkight will start in london again and reach Delhi.
4. And I will catch a flight in Delhi and reach vizag.

* Things I would like to carry:
* Toiletries:
  * Tooth brush
  * Sanitizer
  * Perfume
* Makeup bag
  * Bronzer
  * lipstick
  * Highlighter
* Snacks
    * Fanta
    * cocacola
    * Biscuits

**[AboutMe.md](AboutMe.md)**

---

# Food I suggest to others
I will create a table with 4 food items that I absolutely love. They are pizza, pasta, biryani, vanilla cake.

|food item|location|cost|
|---|---|---|
|pizza|pizza hut|6$|
|pasta|FSM|5$|
|biryani|paradise|10$|
|vanilla cake|fresh choice|4$|

---

# Pithy Quotes

>"Little by little, one travels far."-*J.R.R. Tolkien*<br>
>"Mistakes can't be erased, but they move you from your present position."-*Richard Diebenkorn*

---

# SQRT decomposition

>The basic idea of sqrt decomposition is preprocessing. We'll divide the array a into blocks of length approximately n−−√, and for each block i we'll precalculate the sum of elements in it b[i].

[Click Here to know more](https://en.wikipedia.org/wiki/SQRT_meldabe_decomposition)

```

// input data
int n;
vector<int> a (n);

// preprocessing
int len = (int) sqrt (n + .0) + 1; // size of the block and the number of blocks
vector<int> b (len);
for (int i=0; i<n; ++i)
    b[i / len] += a[i];

// answering the queries
for (;;) {
    int l, r;
  // read input data for the next query
    int sum = 0;
    for (int i=l; i<=r; )
        if (i % len == 0 && i + len - 1 <= r) {
            // if the whole block starting at i belongs to [l, r]
            sum += b[i / len];
            i += len;
        }
        else {
            sum += a[i];
            ++i;
        }
}
```

[Code Source](https://cp-algorithms.com/data_structures/sqrt_decomposition.html)






