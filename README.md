What is the result of each of the following:

    >>> "Python"[1]
    >>> "Strings are sequences of characters."[5]
    >>> len("wonderful")
    >>> "Mystery"[:4]
    >>> "p" in "Pineapple"
    >>> "apple" in "Pineapple"
    >>> "pear" not in "Pineapple"
    >>> "apple" > "pineapple"
    >>> "pineapple" < "Peach"

Modify:

    prefixes = "JKLMNOPQ"
    suffix = "ack"

    for letter in prefixes:
        print(letter + suffix)

so that Ouack and Quack are spelled correctly.

Encapsulate

    fruit = "banana"
    count = 0
    for char in fruit:
        if char == "a":
            count += 1
    print(count)

in a function named count_letters, and generalize it so that it accepts the string and the letter as arguments. Make the function return the number of characters, rather than print the answer. The caller should do the printing.

Now rewrite the count_letters function so that instead of traversing the string, it repeatedly calls the find method, with the optional third parameter to locate new occurrences of the letter being counted.

Assign to a variable in your program a triple-quoted string that contains your favourite paragraph of text — perhaps a poem, a speech, instructions to bake a cake, some inspirational verses, etc.

Write a function which removes all punctuation from the string, breaks the string into a list of words, and counts the number of words in your text that contain the letter “e”. Your program should print an analysis of the text like this:

    Your text contains 243 words, of which 109 (44.8%) contain an "e".

Print a neat looking multiplication table like this:

            1   2   3   4   5   6   7   8   9  10  11  12
      :--------------------------------------------------
     1:     1   2   3   4   5   6   7   8   9  10  11  12
     2:     2   4   6   8  10  12  14  16  18  20  22  24
     3:     3   6   9  12  15  18  21  24  27  30  33  36
     4:     4   8  12  16  20  24  28  32  36  40  44  48
     5:     5  10  15  20  25  30  35  40  45  50  55  60
     6:     6  12  18  24  30  36  42  48  54  60  66  72
     7:     7  14  21  28  35  42  49  56  63  70  77  84
     8:     8  16  24  32  40  48  56  64  72  80  88  96
     9:     9  18  27  36  45  54  63  72  81  90  99 108
    10:    10  20  30  40  50  60  70  80  90 100 110 120
    11:    11  22  33  44  55  66  77  88  99 110 121 132
    12:    12  24  36  48  60  72  84  96 108 120 132 144

Write a function that reverses its string argument, and satisfies these tests:


    test(reverse("happy") == "yppah")
    test(reverse("Python") == "nohtyP")
    test(reverse("") == "")
    test(reverse("a") == "a")

Write a function that mirrors its argument:


    test(mirror("good") == "gooddoog")
    test(mirror("Python") == "PythonnohtyP")
    test(mirror("") == "")
    test(mirror("a") == "aa")

Write a function that removes all occurrences of a given letter from a string:


    test(remove_letter("a", "apple") == "pple")
    test(remove_letter("a", "banana") == "bnn")
    test(remove_letter("z", "banana") == "banana")
    test(remove_letter("i", "Mississippi") == "Msssspp")
    test(remove_letter("b", "") = "")
    test(remove_letter("b", "c") = "c")

Write a function that recognizes palindromes. (Hint: use your reverse function to make this easy!):


    test(is_palindrome("abba"))
    test(not is_palindrome("abab"))
    test(is_palindrome("tenet"))
    test(not is_palindrome("banana"))
    test(is_palindrome("straw warts"))
    test(is_palindrome("a"))
    # test(is_palindrome(""))    # Is an empty string a palindrome?

Write a function that counts how many times a substring occurs in a string:

  

    test(count("is", "Mississippi") == 2)
    test(count("an", "banana") == 2)
    test(count("ana", "banana") == 2)
    test(count("nana", "banana") == 1)
    test(count("nanan", "banana") == 0)
    test(count("aaa", "aaaaaa") == 4)

Write a function that removes the first occurrence of a string from another string:

   
    test(remove("an", "banana") == "bana")
    test(remove("cyc", "bicycle") == "bile")
    test(remove("iss", "Mississippi") == "Missippi")
    test(remove("eggs", "bicycle") == "bicycle")

Write a function that removes all occurrences of a string from another string:

   
    test(remove_all("an", "banana") == "ba")
    test(remove_all("cyc", "bicycle") == "bile")
    test(remove_all("iss", "Mississippi") == "Mippi")
    test(remove_all("eggs", "bicycle") == "bicycle")
