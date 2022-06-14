# my-tests
### chilliSentencee [every programmer ought to write tests; these ones are so very special]

- this test was written somewhere about year-eighth-ago. modification time says 13th of may 2014.
- i produce a lot of discarded code during developing my applications (i mean i write tests oftenly).
- i am going to put some special stuff into this repository.
- this particular one is of very high value for me [i am quiet sentimental].
- ![locality_of_reference_(clean)_test](https://user-images.githubusercontent.com/98284211/173679067-76278735-7d0c-4074-a804-4785cc58a1da.svg)

---
- ### here is the code:
>```
>#_a_learning_test_to_check_a_reference_locality_
>#
>#_a_syntax_of_a_language_force_thou_to_declare_
>#_variables_outside_a_function_see_
>learn test $mockingBird, $penguin, $counter, $chilliSentencee, $guess {
>#   $penguin = " singer " it is wrong exception will be
>#             not raised value will be empty (see_below*)
>   $number = 0
>   forward 10
>   print $chilliSentencee
>   if $counter { $number = $number + 1 }
>   $guess = $number
>   if $counter { $chilliSentencee = $penguin }
>   if not $number {
>    $chilliSentencee = $mockingBird + $chilliSentencee
>    }
>    else {
>#_next_string_is_local_it_will_be_evaluated_outside_this_call_*only*_
>     $chilliSentencee = $penguin
>     forward 20
>     message " what is it chilli willy "
>     forward 10
>#_and_this_kind_of_reference_calls_to_$variable_*_with_*old_value*_
>#    print ( $mockingBird + "and" + $chilliSentencee + "are " + $number )
>     }
>   }
>#
>#an_interface
>$counter = false
>$guess = 0
>$penguin = " singer "
>#$penguin = "" default value --to raise an exception not
>$chilliSentencee = $penguin
>reset
>go 10, 300
>penup
>message " here is a mocking bird be aware please "
>$mockingBird = " #scratchie * * * "
>print $mockingBird
>#
>message " here chilli willy did appeared yet "
>forward 20
>test $mockingBird, $penguin, $counter, $chilliSentencee, $guess
>#
>forward 10
>message " now they did putted their bags together say it penguin please "
>forward 20
>print $chilliSentencee
>forward 20
>#
>wait 1
>$counter = true 
>test $mockingBird, $penguin, $counter, $chilliSentencee, $guess
># print $number a mistake --it is a local variable
>forward 10
>print ( $mockingBird + "and" + $chilliSentencee + "are " + $guess )
>forward 20
>print $chilliSentencee
>spritehide
>```
---
![locality_of_reference_(clean)_test Screenshot_2022-06-14_22-06-16](https://user-images.githubusercontent.com/98284211/173679957-ce1892a5-3166-4299-b02c-1e18ed702cb8.png)
