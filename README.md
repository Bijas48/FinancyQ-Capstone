<h2 align="center"> FinancyQ - Manage Your Money, Achieve Your Dreams </h2> 
<br>
<p>Do you want to manage your personal finances more effectively? Meet FinancyQ, a mobile app created to help you master personal finance management. With FinancyQ, you can track your expenses, create budgets, and achieve your long-term financial goals with ease.

Why FinancyQ? Because we understand the financial challenges that are often faced, especially by younger generations such as Gen Z. We have integrated comprehensive income and expense management, innovative authentication methods such as email, and additional functions such as educational cards and PDF reports.</p>
<br>

## Team Member C241-PS355
<div align="center">

| Bangkit ID |               Name               |   Learning Path    |                 Campus                   |
|:----------:|:--------------------------------:|:------------------:|:----------------------------------------:|
|M299D4KX1433| Alya Sahrani                     | Machine Learning   | Universitas Pendidikan Indonesia         |
|M006D4KY2028| Dinar Ferdiansyah                | Machine Learning   | Universitas Brawijaya                    |
|M001D4KY2321| Muhammad Yasir Amri              | Machine Learning   | Institut Pertanian Bogor                 |
|C299D4KY1212| Adrian Kusuma Widjaja Kardana    | Cloud Computing    | Universitas Pendidikan Indonesia         |
|C262D4KY0345| Farhan Nurhidayah                | Cloud Computing    | Universitas Muhammadiyah Prof Dr Hamka   |
|A272D4KY3575| M.Fiqry Septiawan                | Mobile Development | Universitas Muslim Indonesia             |
|A299D4KX3768| Aisyah Husna Alifah              | Mobile Development | Universitas Pendidikan Indonesia         |

</div>

## Screenshots

untuk gambar
<br>

## Cloud Computing Infrastructure
![Design Infra](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/FinancyQ-Architecture.PNG)

## Database Design
![Design database](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/ERD-FinancyQ.PNG)

<br/>

## FinancyQ-API Reference
### Authentications
|Endpoint              |Method  | Parameter          | Authorization  | Description                                   |
|:---------------------|:-------| :------------------| :------------- | :---------------------------------------------|
| `/signup`            |POST    | `application/json` |                | Register user                                 |
| `/verifyotp`         |POST    | `application/json` |                | Verify Token user from email                  |
| `/login`             |POST    | `application/json` |                | Login user                                    |
| `/logout`            |POST    | `application/json` |                | Logout user                                   |

### Users
|Endpoint                |Method  | Parameter          | Authorization  | Description                                   |
|:-----------------------|:-------| :------------------| :------------- | :---------------------------------------------|
| `/users:username`      |GET     | `application/json` | `Bearer Token` | Get a specific user                           |
| `/users:username`      |POST    | `application/json` | `Bearer Token` | Change Data of user                           |
| `/users:username`      |DELETE  | `application/json` | `Bearer Token` | Delete Account user                           |

### Transactions
|Endpoint                      |Method  | Parameter          | Authorization  | Description                           |
|:-----------------------------|:-------| :------------------| :------------- | :-------------------------------------|
| `/products-catalog`          | GET    | `application/json` | `Bearer Token` | Get all product catalog               |
| `/product-category/category` | GET    | `application/json` | `Bearer Token` | Get product catalog based on category |
| `/product-id/id`             | GET    | `application/json` | `Bearer Token` |GET product by Id                      |
| `/product-catalog`           | POST   | `application/json` | `Bearer Token` |Add Product for Catalog                |
| `/product-catalog/id`        | PUT    | `application/json` | `Bearer Token` |Update Product Catalog                 |


### Education Content
|Endpoint                 |Method  | Parameter          | Authorization  | Description                                   |
|:------------------------|:-------| :------------------| :------------- | :---------------------------------------------|
| `/education-content`    |GET     | `application/json` |                | Get list of education content                 |
| `/education-content/:id`|GET     | `application/json` |                | Get a specific of education content           |

