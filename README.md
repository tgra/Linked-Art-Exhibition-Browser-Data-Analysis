# linked-art-data-analysis-app

Data analysis app for linked art exhibition data using jupyter notebooks and mercury 


## Mercury
https://github.com/mljar/mercury



params:
    exhibition_data_type:
        input: select
        label: Data to display
        value: all
        choices: [all, MoMA, non-MoMA]
        multi: False 
    organisation:
        input: select
        label: Organisation
        choices: [The City Gallery,Judson Gallery,Reuben Gallery,Brata Gallery,Green Gallery,Hansa Gallery,Tanager Gallery,MoMA PS1,The Museum of Modern Art]
    selected_year:
        input: text
        label: Enter year to view exhibition per month in selected year
        value:
    gender:
        input: select
        label: gender
        value: all
        choices: [all, Male, Female]