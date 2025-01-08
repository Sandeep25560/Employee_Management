# Employee Management with ASP.NET Core 5 + ReactJS

## **Overview**
This project demonstrates a full-stack Employee Management system built using **ASP.NET Core 5** for the backend and **ReactJS** for the frontend. It showcases a modular, reusable, and scalable architecture for handling CRUD operations with a modern UI.

---

## **Project Structure**
- **EmployeeManager.API**:  
  Backend implementation using the **ASP.NET Core 5 Web API** template. It integrates with a Docker container of **MS SQL Server 2019**, ensuring cross-platform compatibility for database management.
  
- **EmployeeManager.Web**:  
  Frontend implementation using the **ReactJS** framework. It leverages **Chakra-UI** for component styling and **Axios** as the HTTP client for seamless API communication.

---

## **Features**
- **CRUD Operations**:  
  Comprehensive implementation for creating, reading, updating, and deleting employee records.
  
- **Code/Component Reusability**:  
  Modular codebase enabling efficient reuse of components and business logic.

- **Validation**:  
  - **Server-side Validation**: Ensures data integrity at the backend.  
  - **Client-side Validation**: Provides immediate feedback to users.

- **React Routing**:  
  Enables navigation between views such as employee lists, forms, and details.

---

## **Technology Stack**
- **Backend**:  
  - ASP.NET Core 5 Web API  
  - MS SQL Server 2019 (Dockerized)

- **Frontend**:  
  - ReactJS  
  - Chakra-UI (Styling)  
  - Axios (HTTP Client)

- **Tools & Platforms**:  
  - Docker  
  - Visual Studio / Visual Studio Code

---

## **Setup Instructions**

### **Backend (EmployeeManager.API)**
1. **Prerequisites**:
   - .NET SDK 5.0 or later
   - Docker installed and running

2. **Steps**:
   - Navigate to the `EmployeeManager.API` directory.
   - Start the MS SQL Server Docker container:
     ```bash
     docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=YourStrongPassword!' -p 1433:1433 -d mcr.microsoft.com/mssql/server:2019-latest
     ```
   - Update the connection string in `appsettings.json` to point to the running Docker container.
   - Run the API:
     ```bash
     dotnet run
     ```

### **Frontend (EmployeeManager.Web)**
1. **Prerequisites**:
   - Node.js and npm installed

2. **Steps**:
   - Navigate to the `EmployeeManager.Web` directory.
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the development server:
     ```bash
     npm start
     ```

---

## **How to Use**
1. **Add Employee**: Navigate to the "Add Employee" page to create a new record.
2. **View Employees**: Browse the list of all employees with paginated results.
3. **Edit Employee**: Update existing employee details using the "Edit" option.
4. **Delete Employee**: Remove an employee record with a single click.

---

## **Screenshots**
Include screenshots or GIFs of the application for better visualization:
1. Employee List View  
2. Add/Edit Employee Form  
3. Validation Error Messages  

---

## **Contributing**
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
