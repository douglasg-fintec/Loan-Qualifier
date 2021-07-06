# Loan-Qualifier 

Extend the CLI of an existing application to prompt the user to save the qualifying loans as a new CSV file so that the results can be shared as a spread sheet.


## Technologies

### Programming  Language
Python 3.9

### Libraries and Frameworks

**fire 0.4.0** - Python Fire is a library for automatically generating command line interfaces (CLIs) from absolutely any Python object.
https://google.github.io/python-fire/guide/

**questionary 1.9.0** - A Python library for effortlessly building pretty command line interfaces 
https://questionary.readthedocs.io/en/stable/

**pytest 6.2.3**  - The pytest framework makes it easy to write small to complex functional testing for applications and libraries.
https://docs.pytest.org/en/stable/

**csv 0.14.1** - csv file reading and writing library   
https://docs.python.org/3/library/csv.html

**pathlib 3.4** - object oriented file system paths 
https://docs.python.org/3/library/pathlib.html

---

## Installation Guide
In order to run the Loan-Query application you must install the folloing depenedencies. They can each be installed with pip by runbning the following commands:

>"pip install fire"

>"pip install questionary"

>"pip install pytest"

>"pip install csv"

>"pip install pathlib"

---

## Examples

This code block outlines the basic flow of the application logic

# The main function 
def run():
    """The main function for running the script."""

    # Load the latest Bank data
    bank_data = load_bank_data()

    # Get the applicant's information
    credit_score, debt, income, loan_amount, home_value = get_applicant_info()
    
    # Find qualifying loans
    qualifying_loans = find_qualifying_loans(
        bank_data, credit_score, debt, income, loan_amount, home_value
    )

    # Save qualifying loans
    save_qualifying_loans(qualifying_loans)

---

## Usage

### Run the CLI
Run the CLI
Now open your terminal and navigate to your project directory using the cd command. 
Then run your CLI with the following code:

>"python app.py"

https://user-images.githubusercontent.com/85652516/124547086-36223380-ddf1-11eb-9d43-78cde4663fd6.png

## Contributors

Gregory Douglas
gregory.w.douglas@cheopsconsulting.com
twitter: gregorywdouglas
LinkedIn: gregorywdouglas

---

## License

MIT
