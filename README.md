# ASP.NET Core MVC WebApp  
### This repository contains the assignments for the **ASP.NET Fundamentals** course @ SoftUni.  

[![C#](https://img.shields.io/badge/Made%20with-C%23-239120.svg)](https://learn.microsoft.com/en-us/dotnet/csharp/)
[![.NET](https://img.shields.io/badge/.NET-5C2D91.svg)](https://dotnet.microsoft.com/)
[![ASP.NET Core MVC](https://img.shields.io/badge/ASP.NET%20Core-MVC-512BD4.svg)](https://github.com/dotnet/aspnetcore)

---
## 📖 Introduction  
Build an ASP.NET Core MVC application using the Model-View-Controller pattern. This project provides hands-on experience in creating, configuring, and managing simple MVC applications with the ASP.NET framework.  

## 🔧 Prerequisites  
Ensure you have:  
- .NET 6.0 SDK or later  
- Visual Studio 2022 or Visual Studio Code  

## 🚀 Getting Started  
### 1️⃣ Create a New ASP.NET Core MVC Project  
- Open Visual Studio 2022 or Visual Studio Code.  
- Select **Create a New Project**.  
- Choose **ASP.NET Core Web App (Model-View-Controller)**.  
- Set the project name and directory.  
- Target framework: **.NET 6.0 (LTS)**.  
- Click **Create**.  

### 2️⃣ Add Controllers and Views  
- Add a controller in the `Controllers` folder:  
  **Add** > **Controller** > **MVC Controller - Empty**.  
- Add views in the `Views` folder, matching the controller names.  

### 3️⃣ Configure Routing  
Set up routing in `Startup.cs` or `Program.cs`:  
```csharp
app.UseRouting();
app.UseEndpoints(endpoints =>
{
    endpoints.MapControllerRoute(
        name: "default",
        pattern: "{controller=Home}/{action=Index}/{id?}");
});
```
This configuration defines the default route pattern where `HomeController` and its `Index` action will be accessed as the default page.

### 4️⃣ Run the Application
To start the project, either press `F5` or click on the **Run** button in Visual Studio. Your application should launch in a browser window at `https://localhost:{port}`. Use this link to access the MVC pages you have built.

## ⚙️ Functionalities
### 🏠 Home Page
The **Home Page** is the main entry point of the application. To begin, a specific action needs to be defined within the application to handle requests for this page. In this case, we’ll create an action called Index. Next, a custom view will be added where a welcoming message and simple content will be displayed. The home page will be set as the default landing page, ensuring that it is the first page users see when they visit the application.

### ℹ️ About Page
An **About Page** provides an opportunity to describe the purpose of the application or give background information about its developers. To create this, a new action is added specifically for the About Page. A corresponding view will be created to house the content. Once the page is set up, a link will be added on the home page to make it easily accessible to users.

### 📞 Contact Page
The **Contact Page** allows users to reach out with their inquiries or comments. To build this page, both an action and a view are created. On this page, a form will be included where users can input their name, email, and a message. Basic validation ensures that users fill in all the required fields before submitting the form, making it a functional and interactive element of the application.

### 🔗 Navigation Links
To ensure easy access to various parts of the site, navigation links will be added. These links, placed in a shared layout that appears on every page, will guide users to the Home, About, and Contact pages. This common navigation bar enhances the overall user experience by allowing visitors to quickly jump between the different sections of the site.

### 🛍️ "All Products" Page
The **All Products Page** is where users can browse through the complete list of products. Multiple viewing options will be available, including the ability to see the list of products in **JSON** format or as **Plain Text**. Users can also download the product list as a text file. Additionally, a search function will be implemented to help users filter through the products, and an alternative URL will be provided to access this page.

### 💬 Simple Chat ASP.NET Core MVC App
A simple, real-time **Chat Application** will be built within the site. This feature will enable users to send and receive messages instantly, mimicking live communication. A technology such as **SignalR** will be used to manage the real-time message updates, ensuring smooth interaction between users.

### ✂️ Text Splitter App
A **Text Splitter** Tool will be developed as part of the app's functionality. This tool takes user input and splits it into smaller parts, such as individual words or sentences. It will be useful for analyzing or processing text in a structured way

### 🎨 Styling the Pages
The visual appeal of the site will be improved by adding CSS styles. A `wwwroot` folder will be created to house the necessary style files. These styles will be applied consistently across all pages, ensuring that the site has a cohesive look. The shared layout file will be styled to ensure that common elements, like navigation links, appear uniform on every page.
  
## 💡 Additional Resources
For more advanced features and functionalities, refer to the official [ASP.NET Core documentation](https://docs.microsoft.com/en-us/aspnet/core/)

## 📜 License
This project is licensed under the [MIT License](LICENSE). See the [LICENSE](LICENSE) file for details.

## 📬 Contact
For any questions or suggestions, please open an issue in the repository.
