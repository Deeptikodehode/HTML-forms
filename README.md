<head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Form</title>
    <!-- To add the internal CSS< -->
    <style>
      /*Set the width of the body */
      body {
        width: 55%;
        margin: 20px auto;
        padding: 20px;
      }
      /*Set the input fields in the form  */

      /* To set the text field*/
      input[type="text"] {
        width: 50%;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-size: medium;
      }
      /* Change the color when mouse is over on it */
      input[type="text"]:focus {
        background-color: rgb(206, 234, 152);
      }
      /* To set the Email field*/
      input[type="email"] {
        width: 50%;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-size: medium;
      }
      /* Change the color when mouse is over on it */
      input[type="email"]:focus {
        background-color: rgb(206, 234, 152);
      }
      /* To set the Password field*/
      input[type="password"] {
        width: 45%;
      }
      /* Change the color when mouse is over on it */
      input[type="password"]:focus {
        background-color: rgb(206, 234, 152);
      }
      /* To set the calander field*/
      input[type="date"] {
        width: 45%;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-size: medium;
      }
      /* Change the color when mouse is over on it */
      input[type="date"]:focus {
        background-color: rgb(206, 234, 152);
      }
      select {
        width: 35%;
        text-align: center;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-size: medium;
      }
      /* Change the color when mouse is over on it */
      select:hover {
        background-color: rgb(206, 234, 152);
      }
      /* To set the submit button field*/
      input[type="submit"] {
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-weight: bold;
        margin: 0px 200px;
        background-color: rgb(241, 51, 51);
        color: white;
        border-radius: 10px;
        padding: 5px 20px;
      }
      /* To set the Section of field*/
      legend {
        background-color: rgb(38, 88, 38);
        color: white;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-weight: bold;
        text-align: center;
        border: 2px solid;
        padding: 5px 20px;
      }
      /* To set the background of the label and input field*/
      fieldset {
        background-color: rgb(190, 239, 190);
      }
      /* To set the lebel field*/
      label {
        margin: 20px;
        font-family: Arial, Helvetica, sans-serif;
      }
    </style>
  </head>
  <body>
    <form>
      <!-- To Set the personalia part -->
      <fieldset>
        <legend>Personalia</legend>

        <label for="fName">First Name</label>
        <input
          type="text"
          id="fName"
          name="fName"
          placeholder="Your name"
          required
        /><br /><br />
        <label for="lName">Last Name</label>
        <input type="text" id="lName" name="lName" /><br /><br />
        <label for="dof">Date of Birth</label>
        <input type="date" id="dof" name="dateOfBirth" /><br /><br />
        <label for="gender">Gender</label>
        <input type="radio" id="male" name="Gender" value="Male" />
        <label for="male">Male</label>
        <input type="radio" id="female" name="Gender" value="Female" />
        <label for="female">Female</label><br /><br />
        <label for="city">City</label>
        <select name="City" id="city">
          <option value="selected" disabled selected>----Select----</option>
          <option value="Bergen">Bergen</option>
          <option value="Oslo">Oslo</option>
          <option value="Stavanger">Stavanger</option>
        </select>
      </fieldset>
      <!-- To set the login part -->
      <fieldset>
        <legend>Login Details</legend>
        <label for="email">Email</label>
        <input type="email" id="email" name="Email" required /><br /><br />
        <label for="pwd">Password</label>
        <input
          type="password"
          id="pwd"
          name="Password"
          minlength="8"
          maxlength="12"
          required
        /><br /><br />
        <input type="submit" value="Submit" />
      </fieldset>
    </form>
  </body>
