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

# APK App
[Click Here](https://drive.google.com/drive/folders/1CsYPlkcOE8taGhDN0y322GHwObfhY_sW?usp=sharing)

## Screenshots
![SS1](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/SS_3app.PNG)
![SS2](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/SS_4app.PNG)
![SS1](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/SS_5app.PNG)
![SS2](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/SS_6app.PNG)
<br>
## Machine Learning Model
[Machine Learning Overview](https://colab.research.google.com/drive/1Hg4-T_aGRaU3wlkQsK8aSfOYF-Gg9ESo?usp=sharing#scrollTo=NtYSbOo43ZMT)

## Cloud Computing Infrastructure
![Design Infra](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/FinancyQ-Architecture.PNG)

## Database Design
![Design database](https://github.com/Bijas48/FinancyQ-Capstone/blob/main/assets/ERD-FinancyQ.PNG)

<br/>

## FinancyQ-API Reference

Our Base URL : `https://financyq-api-app.web.app/`\
[Postman FinancyQ API documentation](https://documenter.getpostman.com/view/34627628/2sA3XLDitK)
Feel Free to Test Our API


### Authentications
|Endpoint              |Method  | Content-Type       | Authorization  | Description                                   |
|:---------------------|:-------| :------------------| :------------- | :---------------------------------------------|
| `/signup`            |POST    | `application/json` |                | Register user                                 |
| `/verifyotp`         |POST    | `application/json` |                | Verify Token user from email                  |
| `/login`             |POST    | `application/json` |                | Login user                                    |
| `/logout`            |POST    | `application/json` |                | Logout user                                   |

### Users
|Endpoint                |Method  | Content-Type       | Authorization  | Description                                   |
|:-----------------------|:-------| :------------------| :------------- | :---------------------------------------------|
| `/users:username`      |GET     | `application/json` | `Bearer Token` | Get a specific user                           |
| `/users:username`      |POST    | `application/json` | `Bearer Token` | Change Data of user                           |
| `/users:username`      |DELETE  | `application/json` | `Bearer Token` | Delete Account user                           |

### Transactions
|Endpoint                                   | Method   |  Content-Type         | Authorization  | Description                                                        |
|:------------------------------------------|:---------| :---------------------| :------------- | :------------------------------------------------------------------|
| `/api/transactions/:userId/export-pdf`    | GET      | `application/json`    | `Bearer Token` | Get Download a PDF of History Transaction a specific user          |
| `/api/transactions/total/:type/:idUser`   | GET      | `application/json`    | `Bearer Token` | Get Total/Sum of `Pemasukan` and `Pengeluaran` value of user       |
| `/api/transactions/:type/:idUser`         | GET      | `application/json`    | `Bearer Token` | Get History transaction of `type` user                             |
| `/api/transactions/:type`                 | POST     | `application/json`    | `Bearer Token` | Create a transaction of the specified `type` user                  |
| `/api/transactions/:type/:id`             | PUT      | `application/json`    | `Bearer Token` | Update a transaction of the specified `type` and `id` transaction  |
| `/api/transactions/:type/:id`             | DELETE   | `application/json`    | `Bearer Token` | Delete a transaction of the specified `type` and `id` transaction  |
| `/api/transactions/classify`              | DELETE   | `multipart/form-data` |                | Scanning Image using model ML                                      |

`type` is params for `pemasukan` or `pengeluaran` to matching based on database`s tables.


### Education Content
|Endpoint                 |Method  | Content-Type       | Authorization  | Description                                   |
|:------------------------|:-------| :------------------| :------------- | :---------------------------------------------|
| `/education-content`    |GET     | `application/json` |                | Get list of education content                 |
| `/education-content/:id`|GET     | `application/json` |                | Get a specific of education content           |

