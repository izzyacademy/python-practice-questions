
## Assignment Number 1

1. Create a function called `calculate_taxes`.

   It accepts the following parameters:

   * `quantity`, like `3`
   * `unit_price`, like `$3.59`
   * A Boolean called `is_taxable`
   * `sales_tax_rate` (between `0.00` and `20.00`)

   It should calculate and return the sales tax if the item is taxable.

2. Create a function called `calculate_subtotal`.

   It accepts the following parameters and returns the subtotal, including the taxes if applicable:

   * `quantity`: an integer
   * `unit_price`: a floating-point number
   * `is_taxable`: a Boolean
   * `sales_tax_rate` (between `0.00` and `20.00`)

## Test Data for `calculate_taxes`

| quantity | unit_price | is_taxable | sales_tax_rate |
| -------: | ---------: | :--------: | -------------: |
|        1 |       1.00 |    False   |         15.00% |
|       10 |     100.00 |    False   |         19.50% |
|      100 |      50.00 |    True    |          6.50% |
|        1 |       1.00 |    True    |         15.00% |
|       25 |      10.00 |    True    |           7.00 |

## Test Data for `calculate_subtotal`

| quantity | unit_price | is_taxable | sales_tax_rate |
| -------: | ---------: | :--------: | -------------: |
|        1 |       1.00 |    False   |         15.00% |
|       10 |     100.00 |    False   |         19.50% |
|      100 |      50.00 |    True    |          6.50% |
|        1 |       1.00 |    True    |         15.00% |
|       25 |      10.00 |    True    |           7.00 |
