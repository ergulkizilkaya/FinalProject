# FinalProject
Bu repo **Yazılım Geliştirici Yetiştirme Kampı**'nda yapılan çalışmaları kapsayan **Final Projesi**'ni içerir.
## :pushpin:Getting Started
N-Katmanlı mimari yapısı ile hazırlanan, northwind veritabanı kullanılarak veri yönetimin yapıldığı,Console arayüzü ile çalışan örnek bir proje. Northwind veritabanı için [Nortwind Sql Code](https://github.com/microsoft/sql-server-samples/blob/master/samples/databases/northwind-pubs/instnwnd.sql)
## :books:Layers
### Entities Layer
Veritabanı nesneleri için oluşturulmuş **Entities Katmanı**'nda **Abstract** ve **Concrete** olmak üzere iki adet klasör bulunmaktadır.Abstract klasörü soyut nesneleri, Concrete klasörü somut nesneleri tutmak için oluşturulmuştur.  
<br>:file_folder:`Abstract`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [IEntity.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/Entities/Abstract/IEntity.cs)
<br> <br> :file_folder:`Concrete`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [Category.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/Entities/Concrete/Category.cs)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [Customer.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/Entities/Concrete/Customer.cs)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [Product.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/Entities/Concrete/Product.cs)  
###  Business Layer
Sunum katmanından gelen bilgileri gerekli koşullara göre işlemek veya denetlemek için oluşturulan **Business Katmanı**'nda **Abstract** ve **Concrete** olmak üzere iki adet klasör bulunmaktadır.Abstract klasörü soyut nesneleri, Concrete klasörü somut nesneleri tutmak için oluşturulmuştur.  
<br>:file_folder:`Abstract`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [IProductService.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/Business/Abstract/IProductService.cs)
<br> <br> :file_folder:`Concrete`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [ProductManager.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/Business/Concrete/ProductManager.cs)  
###  Data Access Layer
Veritabanı CRUD işlemleri gerçekleştirmek için oluşturulan **Data Access Katmanı**'nda **Abstract** ve **Concrete** olmak üzere iki adet klasör bulunmaktadır.Abstract klasörü soyut nesneleri, Concrete klasörü somut nesneleri tutmak için oluşturulmuştur.  
<br>:file_folder:`Abstract`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [ICategoryDal.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/DataAccess/Abstract/ICategoryDal.cs)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [IProductDal.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/DataAccess/Abstract/IProductDal.cs)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up:[ICustomerDal.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/DataAccess/Abstract/ICustomerDal.cs)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [IEntityRepository.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/DataAccess/Abstract/IEntityRepository.cs)
<br> <br> :file_folder:`Concrete`  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:file_folder: `EntityFramework`    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [EfCategoryDal.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/DataAccess/Concrete/EntityFramework/EfCategoryDal.cs)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [EfProductDal.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/DataAccess/Concrete/EntityFramework/EfProductDal.cs)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:page_facing_up: [NorthwindContext.cs](https://github.com/ergulkizilkaya/FinalProject/blob/master/DataAccess/Concrete/EntityFramework/NorthwindContext.cs)  
### :red_circle:Prerequisites
```
EntityFrameworkCore 3.1.11
```

## :pencil2:Authors
* **Ergül Kızılkaya** - [ergulkizilkaya](https://github.com/ergulkizilkaya)
