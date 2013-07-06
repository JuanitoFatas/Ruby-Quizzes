# Ruby Quizzes

# Solutions?

If you find a better solution (or equally good), please open an issue with the question id, e.g.: `RQS-001`.

# Add a Quiz?

Please do so. And please add the quiz in this form: `RQS-xxx` where `xxx` is a 3-digit integer.

## RQS-001

```ruby
# Input:
#
# str_perm_char("yes")
#
# Output:
#
# ["yes", "yeS", "yEs", "yES", "Yes", "YeS", "YEs", "YES"]
```

## RQS-002

```ruby
# Input:
#
# str_perm("abc")
#
# Output
#
# ["abc", "acb", "bac", "bca", "cab", "cba"]
```

## RQS-003

```ruby
# Input
#
# truth_table(bits: 3)
#
# Output
#
# [[0, 0, 0],
#  [0, 0, 1],
#  [0, 1, 0],
#  [0, 1, 1],
#  [1, 0, 0],
#  [1, 0, 1],
#  [1, 1, 0],
#  [1, 1, 1]]
```

## RQS-004

source: http://ruby-china.org/topics/1504

Implement a `rand_split` method, modify an array into array with `max_element` elements.

```ruby
rand_split(array, max_element)
pry> p rand_split (0..10).to_a, 3
pry> [[0], [1,2], [3, 4, 5], [6, 7], [8], [9, 10]]
```

__BONUS:__ add unit test or minitest.

## RQS-005

source: http://ruby-china.org/topics/1517

Given two parameters:

  - targeting integer, e.g. `5`
  - an array with numbers, e.g. `[-1, 0, 1, 2, 3, 4]`

__Objective:__

Use the numbers in array (only used once) in which their sum is equal to targeting integer (`+`). Return an array which satisfy this constraint.

E.g.:

targeting integer: `5`

Given array: `[-1, 0, 1, 2, 3, 4]`

Output will be:

    [1, 4], [2, 3], [-1, 2, 4], [0, 1, 4], [0, 2, 3], [-1, 0, 2, 4], [-1, 1, 2, 3]