# Assignment

writing the script in Cypress using BDD frame work
Feature file 
feature :-End to end data validation by inserting the values
   Scenario:Inserting the some random data into input text box
   Given:I open the provided url
   when I click on the table data
   And it should open text box
   Then need to enter the data and click on refresh table

Step defnition file:-

    describe('My first test case',()=>
    {
     it('test case',()=>
     {
        cy.visit("https://testpages.herokuapp.com/styled/tag/dynamic-table.html");
        cy.get("#add").click();
        cy.get("#jsondata").type({"name":"Sara", "age" : 42, "gender": "female"}, {"name": "Conor", "age" : 40, "gender": "male"}, {"name":
                "Jennifer", "age" : 42, "gender": "female"}]
       cy.get('.styled-click-button').click();
       
    })
     })
