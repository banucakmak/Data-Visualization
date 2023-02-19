# Data-Visualization

There are 3 packages to import before starting a data visualization.

![image](https://user-images.githubusercontent.com/122751581/219972009-1c091502-efce-4f18-b841-654cab8cd0bc.png)

numpy automatically does the computing. 

It also provides a range of functions for performing operations on these arrays, such as mathematical, logical, shape manipulation, and much more

### Creating x,y,z arrays.
42 is useful as a random seed value because we want to have the same numbers every time we run the code.

![image](https://user-images.githubusercontent.com/122751581/219972216-e8e5fdc1-1521-4c8e-a929-ec274a5bfdc2.png)

![image](https://user-images.githubusercontent.com/122751581/219972358-2f96c10a-8a0a-49c5-a2d8-812b5f36994f.png)

 With the use of matloplib library, there are various ways of visualizing the data
![image](https://user-images.githubusercontent.com/122751581/219972531-e9017cad-b9b3-4c0f-b89c-76779de2d1d2.png)

plt.savefig("x.png",dpi=300) helps us to save the visual data as an image file.

![image](https://user-images.githubusercontent.com/122751581/219973342-1c49b53b-7512-4064-8fb8-b4e87f70bcb8.png)

## Let's analyse a real data set!
  Data set from 3 branches of a supermarket.
  
 ### Some EDA.
  
  ![image](https://user-images.githubusercontent.com/122751581/219974050-88f28564-0c41-4bbe-b669-ab89e47ec690.png)

df.info()
df.isnull().sum()
df.describe()
df.corr()


![image](https://user-images.githubusercontent.com/122751581/219974122-009a9d80-860c-47e3-971a-fa59e69d94e9.png)

![image](https://user-images.githubusercontent.com/122751581/219974182-714e4603-e241-49d3-9df2-d719504286a6.png)

### It seems that apprxmately 250 USD is spent on average

![image](https://user-images.githubusercontent.com/122751581/219974251-bf039d6d-25d7-4f4e-90fa-96a5dd117223.png)

![image](https://user-images.githubusercontent.com/122751581/219974290-1b1d992d-cab9-4a72-9975-48bbc847d338.png)

### Gender and product distribution

![image](https://user-images.githubusercontent.com/122751581/219974326-e7a0272a-687e-4d89-b1ed-a39a1bf34db5.png)

### Each variable in the DataFrame is plotted against every other variable


## Let's see which days and months sales are the highest

![image](https://user-images.githubusercontent.com/122751581/219974523-46b030e1-f48c-4b93-a329-765fe6eab467.png)

### "Date" column datas were object, so were converted to datetime64[ns]  

--Some feature engineering

![image](https://user-images.githubusercontent.com/122751581/219974650-a139d87e-29ab-4e46-bef5-ab70ac0f6451.png)


### We can look through sales according to months, days, cities and customer type by "countplot" command. 

sns.countplot(x=df["month_name"])
sns.countplot(x=df["weekday"])
sns.countplot(x=df["City"])
sns.countplot(x=df["Customer type"])


![image](https://user-images.githubusercontent.com/122751581/219974782-33eda7d8-ca29-4550-b83f-5e63701771cc.png)

### Here we see, count of products in each branch.

![image](https://user-images.githubusercontent.com/122751581/219974804-1e67cbd0-5eda-4b7b-a8d0-04dae1e0d9e8.png)

### Different from countplot we can also have a comparitive data plot representing the mean value of gross income to product line.

![image](https://user-images.githubusercontent.com/122751581/219974814-c6929dbe-d901-45ad-b57f-c6dd28207272.png)

### With this very simple code, we can see what is the shopping behavior of men and women according to branch category and months by the variables of hour and quantity.
