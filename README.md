# Studi/o Access Ally  

## Studio inventory management  

### Intro/Setup
Thank you for checking out our studio management app. This app allows a studio to add their equipment, allows user to submit rental forms, and admins to accept or deny those rental forms. To view the app, you can either <a href="https://www.youtube.com/watch?v=G5pu3HzPXZA" target="_blank">check out our presentation here</a>, or follow these instructions. (Note: You must have Visual Studio Community, Microsoft SQL Server Management Studio 18, Visual Studio Code and Node.JS installed)  

1. Clone down the repository
2. Change the directory to Studio-Access-Ally/backend/Studio-Inventory-API and open the .sln file in Visual Studio 
3. This project uses Entity Framework Core, so in the menus, go to Tools > NuGet Package Manager > Package Manager Console and run the command update-database
4. Now you can run the API by clicking the ► IIS Express button at the top of the window. This will open the API in a browser window, and you will see some JSON data (EquipmentList in the URL). Feel free to minimize this window, but don't close the window.
5. Next, in the command line, change the directory to Studio-Access-Ally/frontend
      * Run the following command
        ```
        npm install webpack webpack-dev-server webpack-cli --save-dev
        ```
3. Now run the command `npm start` to start up the application.

### What you can do:
- See a list of equipment and categories
     - Create, read, update, and delete for each of these (based on type of account)
- Admin vs User Logins (WARNING: NOT SECURE. THE PASSWORDS AT THIS TIME ARE NOT ENCRYPTED AND EASILY ACEESSIBLE)
- Rent forms for equipment. While that equipment is out and being used, it is removed from the available list
     - Admin approval of forms is needed in order to update the equipment list
- About us page for the studio using this app as a template (must be updated in code)
