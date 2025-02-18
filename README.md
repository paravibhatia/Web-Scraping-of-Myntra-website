<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h1>Myntra Web Scraper</h1>

<h2>Overview</h2>
<p>This project is a Selenium-based web scraper designed to extract product details from Myntra's beauty and skincare categories. 
It automates the process of collecting key product attributes such as brand, price, skin type, SPF, key ingredients, and formulation. 
The extracted data is stored in a structured CSV format for further analysis. This project was made for dataset extraction for my ongoing project of skin analysis and product recommendation.</p>

<h2>Features</h2>
<ul>
    <li>Scrapes multiple product categories, including moisturizers, cleansers, sunscreens, and more.</li>
    <li>Extracts essential product details such as brand, price, SPF, key ingredients, and formulation.</li>
    <li>Implements pagination handling to collect a predefined number of products from each category.</li>
    <li>Utilizes Selenium's WebDriverWait to ensure smooth and efficient data extraction.</li>
    <li>Saves extracted data in a structured CSV format.</li>
</ul>

<h2>Data Fields</h2>
<table border="1">
    <tr>
        <th>Field Name</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><strong>label</strong></td>
        <td>Product category (e.g., sunscreen, foundation)</td>
    </tr>
    <tr>
        <td><strong>url</strong></td>
        <td>Product page URL</td>
    </tr>
    <tr>
        <td><strong>brand</strong></td>
        <td>Brand name</td>
    </tr>
    <tr>
        <td><strong>name</strong></td>
        <td>Product name</td>
    </tr>
    <tr>
        <td><strong>price</strong></td>
        <td>Product price</td>
    </tr>
    <tr>
        <td><strong>skin type</strong></td>
        <td>Suitable skin type</td>
    </tr>
    <tr>
        <td><strong>spf</strong></td>
        <td>Sun Protection Factor (if applicable)</td>
    </tr>
    <tr>
        <td><strong>concern</strong></td>
        <td>Primary skin concern the product addresses</td>
    </tr>
    <tr>
        <td><strong>concern 2</strong></td>
        <td>Secondary skin concern (if applicable)</td>
    </tr>
    <tr>
        <td><strong>concern 3</strong></td>
        <td>Additional skin concern (if applicable)</td>
    </tr>
    <tr>
        <td><strong>key ingredient</strong></td>
        <td>Key active ingredients in the product</td>
    </tr>
    <tr>
        <td><strong>formulation</strong></td>
        <td>Product formulation type (e.g., gel, cream)</td>
    </tr>
</table>

<h2>Prerequisites</h2>
<p>Ensure the following dependencies are installed before running the script:</p>
<ul>
    <li>Python (>= 3.7)</li>
    <li>Selenium</li>
    <li>Pandas</li>
    <li>Google Chrome (latest version)</li>
    <li>ChromeDriver (compatible with installed Chrome version)</li>
</ul>

<p>To install the required Python libraries, run:</p>
<pre><code>pip install selenium pandas</code></pre>

<h2>Setup and Execution</h2>
<ol>
    <li>Download and install <strong>Google Chrome</strong> if not already installed.</li>
    <li>Download the appropriate <strong>ChromeDriver</strong> for your Chrome version and update the <code>chrome_path</code> in the script.</li>
    <li>Clone this repository:</li>
</ol>
<pre><code>git clone https://github.com/your-username/myntra-web-scraper.git
cd Web-Scraping-of-Myntra-website
</code></pre>
<ol start="4">
    <li>Run the script:</li>
</ol>
<pre><code>python scraper.py</code></pre>
<p>After execution, the extracted data will be saved in <code>result.csv</code>.</p>

<h2>Repository Structure</h2>
<pre>
myntra-web-scraper/
│── scraper.py              # Main script for web scraping  
│── requirements.txt        # Required dependencies  
│── result.csv              # Output file (generated after execution)  
│── README.md               # Project documentation  
</pre>

<h2>Notes</h2>
<ul>
    <li>The script collects data for a predefined set of categories and supports pagination.</li>
    <li>If Myntra updates its website structure, certain elements or class names may need modification.</li>
    <li>Selenium's <code>WebDriverWait</code> is implemented to handle dynamic content loading.</li>
</ul>

<h2>License</h2>
<p>This project is licensed under the MIT License.</p>

<h2>Contact</h2>
<p>For any issues or contributions, please submit a pull request or open an issue in the repository.</p>

</body>
</html>
