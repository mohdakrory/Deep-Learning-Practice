# Automobile mile per gallon prediction

Predict automobile mile per gallon based on given features

## Dataset description

### Source

[Auto-mpg](https://archive.ics.uci.edu/dataset/9/auto+mpg)

### Samples

<table border="1">
  <thead>
    <tr>
      <th>mpg</th>
      <th>cylinders</th>
      <th>displacement</th>
      <th>horsepower</th>
      <th>weight</th>
      <th>acceleration</th>
      <th>model year</th>
      <th>origin</th>
      <th>car name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>18.0000</td>
      <td>8</td>
      <td>307.0000</td>
      <td>130</td>
      <td>3504</td>
      <td>12.0000</td>
      <td>70</td>
      <td>USA</td>
      <td>chevrolet chevelle malibu</td>
    </tr>
    <tr>
      <td>15.0000</td>
      <td>8</td>
      <td>350.0000</td>
      <td>165</td>
      <td>3693</td>
      <td>11.5000</td>
      <td>70</td>
      <td>USA</td>
      <td>buick skylark 320</td>
    </tr>
    <tr>
      <td>18.0000</td>
      <td>8</td>
      <td>318.0000</td>
      <td>150</td>
      <td>3436</td>
      <td>11.0000</td>
      <td>70</td>
      <td>USA</td>
      <td>plymouth satellite</td>
    </tr>
    <tr>
      <td>16.0000</td>
      <td>8</td>
      <td>304.0000</td>
      <td>150</td>
      <td>3433</td>
      <td>12.0000</td>
      <td>70</td>
      <td>USA</td>
      <td>amc rebel sst</td>
    </tr>
    <tr>
      <td>17.0000</td>
      <td>8</td>
      <td>302.0000</td>
      <td>140</td>
      <td>3449</td>
      <td>10.5000</td>
      <td>70</td>
      <td>USA</td>
      <td>ford torino</td>
    </tr>
    <!-- ... (add other rows as needed) ... -->
    <tr>
      <td>27.0000</td>
      <td>4</td>
      <td>140.0000</td>
      <td>86</td>
      <td>2790</td>
      <td>15.6000</td>
      <td>82</td>
      <td>USA</td>
      <td>ford mustang gl</td>
    </tr>
    <tr>
      <td>44.0000</td>
      <td>4</td>
      <td>97.0000</td>
      <td>52</td>
      <td>2130</td>
      <td>24.6000</td>
      <td>82</td>
      <td>Europe</td>
      <td>vw pickup</td>
    </tr>
    <tr>
      <td>32.0000</td>
      <td>4</td>
      <td>135.0000</td>
      <td>84</td>
      <td>2295</td>
      <td>11.6000</td>
      <td>82</td>
      <td>USA</td>
      <td>dodge rampage</td>
    </tr>
    <tr>
      <td>28.0000</td>
      <td>4</td>
      <td>120.0000</td>
      <td>79</td>
      <td>2625</td>
      <td>18.6000</td>
      <td>82</td>
      <td>USA</td>
      <td>ford ranger</td>
    </tr>
    <tr>
      <td>31.0000</td>
      <td>4</td>
      <td>119.0000</td>
      <td>82</td>
      <td>2720</td>
      <td>19.4000</td>
      <td>82</td>
      <td>USA</td>
      <td>chevy s-10</td>
    </tr>
  </tbody>
</table>

> **398 rows × 9 columns**

### Variable information

<table>
  <tr>
    <th>Variable Name</th>
    <th>Role</th>
    <th>Type</th>
    <th>Demographic</th>
    <th>Description</th>
    <th>Units</th>
    <th>Missing Values</th>
  </tr>
  <tr>
    <td>displacement</td>
    <td>Feature</td>
    <td>Continuous</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
  <tr>
    <td>mpg</td>
    <td>Target</td>
    <td>Continuous</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
  <tr>
    <td>cylinders</td>
    <td>Feature</td>
    <td>Integer</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
  <tr>
    <td>horsepower</td>
    <td>Feature</td>
    <td>Continuous</td>
    <td></td>
    <td></td>
    <td></td>
    <td>yes</td>
  </tr>
  <tr>
    <td>weight</td>
    <td>Feature</td>
    <td>Continuous</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
  <tr>
    <td>acceleration</td>
    <td>Feature</td>
    <td>Continuous</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
  <tr>
    <td>model_year</td>
    <td>Feature</td>
    <td>Integer</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
  <tr>
    <td>origin</td>
    <td>Feature</td>
    <td>Integer</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
  <tr>
    <td>car_name</td>
    <td>ID</td>
    <td>Categorical</td>
    <td></td>
    <td></td>
    <td></td>
    <td>no</td>
  </tr>
</table>

## Exploratory data analysis 

### Label mapping of origin 

<table border="1">
  <tr>
    <th>#</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>1</td>
    <td>USA</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Europe</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Japan</td>
  </tr>
</table>

### Checking for duplicates

**Across all features**

0 duplicates

**Across car name, origin, and model year (the same car)**

4 duplicates

<table border="1">
  <thead>
    <tr>
      <th>mpg</th>
      <th>cylinders</th>
      <th>displacement</th>
      <th>horsepower</th>
      <th>weight</th>
      <th>acceleration</th>
      <th>model year</th>
      <th>origin</th>
      <th>car name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>168</td>
      <td>4</td>
      <td>140.0000</td>
      <td>83</td>
      <td>2639</td>
      <td>17.0000</td>
      <td>75</td>
      <td>USA</td>
      <td>ford pinto</td>
    </tr>
    <tr>
      <td>174</td>
      <td>6</td>
      <td>171.0000</td>
      <td>97</td>
      <td>2984</td>
      <td>14.5000</td>
      <td>75</td>
      <td>USA</td>
      <td>ford pinto</td>
    </tr>
    <tr>
      <td>338</td>
      <td>4</td>
      <td>135.0000</td>
      <td>84</td>
      <td>2490</td>
      <td>15.7000</td>
      <td>81</td>
      <td>USA</td>
      <td>plymouth reliant</td>
    </tr>
    <tr>
      <td>342</td>
      <td>4</td>
      <td>135.0000</td>
      <td>84</td>
      <td>2385</td>
      <td>12.9000</td>
      <td>81</td>
      <td>USA</td>
      <td>plymouth reliant</td>
    </tr>
  </tbody>
</table>

> There is two samples for each of these two cars but with different data so it's fine to keep them

### Missing values (missing values in this dataset have '?' as a place holder)

<table border="1">
  <thead>
    <tr>
      <th>mpg</th>
      <th>cylinders</th>
      <th>displacement</th>
      <th>horsepower</th>
      <th>weight</th>
      <th>acceleration</th>
      <th>model year</th>
      <th>origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>6</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
    </tr>
  </tbody>
</table>

> Drop missing values

### Data types

<table border="1">
  <thead>
    <tr>
      <th>Variable</th>
      <th>Data Type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>mpg</td>
      <td>float64</td>
    </tr>
    <tr>
      <td>cylinders</td>
      <td>int64</td>
    </tr>
    <tr>
      <td>displacement</td>
      <td>float64</td>
    </tr>
    <tr>
      <td>horsepower</td>
      <td>object</td>
    </tr>
    <tr>
      <td>weight</td>
      <td>int64</td>
    </tr>
    <tr>
      <td>acceleration</td>
      <td>float64</td>
    </tr>
    <tr>
      <td>model year</td>
      <td>int64</td>
    </tr>
    <tr>
      <td>origin</td>
      <td>object</td>
    </tr>
  </tbody>
</table>

> Horsepower is converted to float while origin is left as an object because it will be mapped back to numbers to calculate correlation

### Visualization of categorical features 

**Bar (count) plot**

![categories_bar_plots](https://github.com/mohdakrory/Deep-Learning-Practice/assets/67663339/ea320f57-ce21-4ab7-b0b3-3f1bb3338c8d)

**Box plot**

![categories_box_plots ](https://github.com/mohdakrory/Deep-Learning-Practice/assets/67663339/5409668b-4c94-4959-abf4-10bb0a8ea4d4)

**Violin plot**

![categories_violin_plots](https://github.com/mohdakrory/Deep-Learning-Practice/assets/67663339/11e9f851-ea16-418c-a62d-d6446d26948e)

**Combined**

![categorical_combined (1)](https://github.com/mohdakrory/Deep-Learning-Practice/assets/67663339/d9476063-4f9b-486d-96c3-fbeaa8063368)

