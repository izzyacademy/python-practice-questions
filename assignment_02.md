
## Assignment Number 2

These are the test data set for the functions from Assignment Number 1

### Test Dataset for calculate_taxes

Use the following array of dictionaries to loop through each element can calculate the taxes for each element and display it

```python

calculate_taxes_test_data = [
    {
        "quantity": 3,
        "unit_price": 12.99,
        "is_taxable": True,
        "sales_tax_rate": 6.50
    },
    {
        "quantity": 8,
        "unit_price": 4.75,
        "is_taxable": False,
        "sales_tax_rate": 7.00
    },
    {
        "quantity": 1,
        "unit_price": 249.99,
        "is_taxable": True,
        "sales_tax_rate": 8.25
    },
    {
        "quantity": 15,
        "unit_price": 2.49,
        "is_taxable": True,
        "sales_tax_rate": 5.50
    },
    {
        "quantity": 4,
        "unit_price": 35.00,
        "is_taxable": False,
        "sales_tax_rate": 10.00
    },
    {
        "quantity": 25,
        "unit_price": 1.99,
        "is_taxable": True,
        "sales_tax_rate": 7.25
    },
    {
        "quantity": 2,
        "unit_price": 599.50,
        "is_taxable": True,
        "sales_tax_rate": 9.00
    },
    {
        "quantity": 50,
        "unit_price": 0.99,
        "is_taxable": False,
        "sales_tax_rate": 6.75
    },
    {
        "quantity": 7,
        "unit_price": 18.40,
        "is_taxable": True,
        "sales_tax_rate": 15.00
    },
    {
        "quantity": 12,
        "unit_price": 7.25,
        "is_taxable": True,
        "sales_tax_rate": 4.50
    },
    {
        "quantity": 100,
        "unit_price": 3.00,
        "is_taxable": False,
        "sales_tax_rate": 19.50
    },
    {
        "quantity": 6,
        "unit_price": 42.80,
        "is_taxable": True,
        "sales_tax_rate": 12.00
    },
    {
        "quantity": 9,
        "unit_price": 10.10,
        "is_taxable": False,
        "sales_tax_rate": 3.25
    },
    {
        "quantity": 30,
        "unit_price": 5.55,
        "is_taxable": True,
        "sales_tax_rate": 8.75
    },
    {
        "quantity": 1,
        "unit_price": 1000.00,
        "is_taxable": True,
        "sales_tax_rate": 20.00
    }
]

```


### Test Dataset for calculate_subtotal

Use the following array of dictionaries to loop through each element can calculate the subtotal for each element and display it


```python
calculate_subtotal_test_data = [
    {
        "quantity": 5,
        "unit_price": 9.99,
        "is_taxable": True,
        "sales_tax_rate": 7.00
    },
    {
        "quantity": 10,
        "unit_price": 15.50,
        "is_taxable": False,
        "sales_tax_rate": 8.50
    },
    {
        "quantity": 2,
        "unit_price": 125.75,
        "is_taxable": True,
        "sales_tax_rate": 6.25
    },
    {
        "quantity": 20,
        "unit_price": 3.25,
        "is_taxable": True,
        "sales_tax_rate": 5.00
    },
    {
        "quantity": 1,
        "unit_price": 799.99,
        "is_taxable": False,
        "sales_tax_rate": 12.50
    },
    {
        "quantity": 14,
        "unit_price": 6.40,
        "is_taxable": True,
        "sales_tax_rate": 9.25
    },
    {
        "quantity": 40,
        "unit_price": 2.15,
        "is_taxable": False,
        "sales_tax_rate": 4.75
    },
    {
        "quantity": 3,
        "unit_price": 89.95,
        "is_taxable": True,
        "sales_tax_rate": 15.00
    },
    {
        "quantity": 75,
        "unit_price": 1.20,
        "is_taxable": True,
        "sales_tax_rate": 3.50
    },
    {
        "quantity": 6,
        "unit_price": 27.30,
        "is_taxable": False,
        "sales_tax_rate": 18.00
    },
    {
        "quantity": 11,
        "unit_price": 13.75,
        "is_taxable": True,
        "sales_tax_rate": 7.75
    },
    {
        "quantity": 100,
        "unit_price": 0.50,
        "is_taxable": True,
        "sales_tax_rate": 2.00
    },
    {
        "quantity": 8,
        "unit_price": 44.99,
        "is_taxable": False,
        "sales_tax_rate": 20.00
    },
    {
        "quantity": 16,
        "unit_price": 11.10,
        "is_taxable": True,
        "sales_tax_rate": 10.50
    },
    {
        "quantity": 4,
        "unit_price": 250.00,
        "is_taxable": True,
        "sales_tax_rate": 6.50
    }
]

```

Assuming monetary results are rounded to **two decimal places**, the expected answers are:

## Expected results for `calculate_taxes_test_data`

```python
calculate_taxes_expected_results = [
    2.53,
    0.00,
    20.62,
    2.05,
    0.00,
    3.61,
    107.91,
    0.00,
    19.32,
    3.92,
    0.00,
    30.82,
    0.00,
    14.57,
    200.00
]
```

| Sample | Quantity | Unit price | Taxable | Tax rate | Expected tax |
| -----: | -------: | ---------: | :-----: | -------: | -----------: |
|      1 |        3 |     $12.99 |   True  |    6.50% |        $2.53 |
|      2 |        8 |      $4.75 |  False  |    7.00% |        $0.00 |
|      3 |        1 |    $249.99 |   True  |    8.25% |       $20.62 |
|      4 |       15 |      $2.49 |   True  |    5.50% |        $2.05 |
|      5 |        4 |     $35.00 |  False  |   10.00% |        $0.00 |
|      6 |       25 |      $1.99 |   True  |    7.25% |        $3.61 |
|      7 |        2 |    $599.50 |   True  |    9.00% |      $107.91 |
|      8 |       50 |      $0.99 |  False  |    6.75% |        $0.00 |
|      9 |        7 |     $18.40 |   True  |   15.00% |       $19.32 |
|     10 |       12 |      $7.25 |   True  |    4.50% |        $3.92 |
|     11 |      100 |      $3.00 |  False  |   19.50% |        $0.00 |
|     12 |        6 |     $42.80 |   True  |   12.00% |       $30.82 |
|     13 |        9 |     $10.10 |  False  |    3.25% |        $0.00 |
|     14 |       30 |      $5.55 |   True  |    8.75% |       $14.57 |
|     15 |        1 |  $1,000.00 |   True  |   20.00% |      $200.00 |

## Expected results for `calculate_subtotal_test_data`

```python
calculate_subtotal_expected_results = [
    53.45,
    155.00,
    267.22,
    68.25,
    799.99,
    97.89,
    86.00,
    310.33,
    93.15,
    163.80,
    162.97,
    51.00,
    359.92,
    196.25,
    1065.00
]
```

| Sample | Quantity | Unit price | Taxable | Tax rate | Expected subtotal |
| -----: | -------: | ---------: | :-----: | -------: | ----------------: |
|      1 |        5 |      $9.99 |   True  |    7.00% |            $53.45 |
|      2 |       10 |     $15.50 |  False  |    8.50% |           $155.00 |
|      3 |        2 |    $125.75 |   True  |    6.25% |           $267.22 |
|      4 |       20 |      $3.25 |   True  |    5.00% |            $68.25 |
|      5 |        1 |    $799.99 |  False  |   12.50% |           $799.99 |
|      6 |       14 |      $6.40 |   True  |    9.25% |            $97.89 |
|      7 |       40 |      $2.15 |  False  |    4.75% |            $86.00 |
|      8 |        3 |     $89.95 |   True  |   15.00% |           $310.33 |
|      9 |       75 |      $1.20 |   True  |    3.50% |            $93.15 |
|     10 |        6 |     $27.30 |  False  |   18.00% |           $163.80 |
|     11 |       11 |     $13.75 |   True  |    7.75% |           $162.97 |
|     12 |      100 |      $0.50 |   True  |    2.00% |            $51.00 |
|     13 |        8 |     $44.99 |  False  |   20.00% |           $359.92 |
|     14 |       16 |     $11.10 |   True  |   10.50% |           $196.25 |
|     15 |        4 |    $250.00 |   True  |    6.50% |         $1,065.00 |



```
