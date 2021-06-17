# refactor 
Homework - UT Coding Boot Camp (Week 1)

## Tasks 
The client, a search engine optimization company, wants a codebase that follows accessibility standards so that their own website will be more recognized by search engines (ironic).

## Steps taken
Many of the basic html elements were replaced with semantic html elements.  Comments were also introduced to help distinguish the different sections of the website.  A website title was added to improve the company image.

The various classes used across the html elements were consolidated to reduce the need for multiple CSS selectors.  The reduction in CSS selectors along with CSS property consolidation vastly reduced the amount of code needed to display the same website before and after.

## Before example
```

.benefits {
    margin-right: 20px;
    padding: 20px;
    clear: both;
    float: right;
    width: 20%;
    height: 100%;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #2589bd;
}

.benefit-lead {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-brand {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-lead h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-brand h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-cost h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-lead img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-brand img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-cost img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

```
## After example
```

/* Benefits sidebar */
.aside-benefits {
    margin-right: 20px;
    padding: 20px;
    clear: both;
    float: right;
    width: 20%;
    height: 100%;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #2589bd;
}

.benefit {
    margin-bottom: 32px;
    color: #ffffff; 
}

.benefit h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}
/* Reduced redundant code in this section from 3 blocks per selector to 1 */

```

## End result
Less overall CSS code and more organized html code, while maintaining the original website design and function.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Contact
Harrison Kidd

harrisonakidd@gmail.com
