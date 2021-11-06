![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Mongoose Recipes

## Introduction

![thai_style_chicken_noodle_soup_pieces_recipe_web](https://user-images.githubusercontent.com/23629340/38369283-ac1bda62-38e7-11e8-9c9b-d9df623f1bc3.jpg)

We've learned how to use Mongoose to create Schemas and then interact with our MongoDB database. In the following exercise, we will practice how to implement this by creating awesome recipes.

## Requirements

- Fork this repo
- Clone this repo

## Submission

- Upon completion, run the following commands:

  ```
  git add .
  git commit -m "Completed lab"
  git push origin master
  ```

- Create Pull Request so your TAs can check up your work.

## Instructions

### Iteration 1 - Recipe Schema


### Iteration 2 - Create a recipe


**To run your code, remember you should use:**

```shell
$ node index.js
```

Tip: When you have successfully created a new recipe (you see it in the database using Compass tool), you might want to comment out this step. The reason for this is that next time when you run `$ node index.js`, it will try to create a new recipe with the same name and you will get an error in the terminal related to the *duplicate keys* - the title should be unique, and the dish with that title already exists in the database.

### Iteration 3 - Insert multiple recipes

We are importing an array of recipes form the `data.json` file. Using the [`Model.insertMany`](https://mongoosejs.com/docs/api.html#model_Model.insertMany) static, you should add the entire array to the database. After inserting the documents, print the title of each recipe to the console.

Tip: Follow the same tip as in the previous step.

### Iteration 4 - Update recipe

Now you should have six different recipes in the database, but there was a mistake in one of them. The **Rigatoni alla Genovese** does not take that long. You should update the `duration` field and set it to **100**. You might want to use the [`Model.findOneAndUpdate`](https://mongoosejs.com/docs/api.html#model_Model.findOneAndUpdate) static. After updating it, print a success message!

### Iteration 5 - Remove a recipe

Oh oh! The `Carrot Cake` is no longer available, so we need to remove it from the database. Using the [`Model.deleteOne`](https://mongoosejs.com/docs/api.html#model_Model.deleteOne) static, remove that recipe from the database and display a success message after doing it!

### Iteration 6 - Close the Database

After completing every task, you need to close the database. Otherwise, the connection will stay open until the node.js process dies. Pay attention to the asynchronicity of the operation. You should only close the connection after everything is done! :wink:

Happy coding! 💙
