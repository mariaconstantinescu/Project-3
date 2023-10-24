# Project-5
Application: A class called Account which will implement functionality to mimic a real-life
scenario for a bank account. In this class, we will implement the following requirements:
1) Attributes List (private):
▪ id representing the ID of the account (use long int type)
▪ owner_name representing the name of the account owner (use string type)
▪ balance representing the current account founds (use float type)
▪ pin representing a secret code of 4 digits that will be used in order to complete transactions
(use int type)
2) Methods List (public):
▪ Setters for attributes: owner_name, pin
▪ Getters for attributes: id, owner_name, balance
▪ Implicit constructor, constructor with parameters, copy constructor (use a message to see the
call)
▪ Destructor (use a message to see the call)
▪ int reset_pin() – Method used to reset the pin. This method will make use of the rand()
function in order to generate a pseudo-random pin each time this function is called. Make sure
that the pin will be capped at a 4 digit number by taking advantage of the modulo operator.
This method will return the newly generated account pin code.
▪ void found_account(float amount) – Method that will be used to found the account. This
method takes as argument the amount of money to be added to the current balance.
▪ float withdraw_money(float amount) – Allows the user to withdraw money from the account.
The transaction will be honored only if the user managed to correctly insert the PIN code (call
to insert_pin() method) , and if the amount to be withdrawn is smaller or equal then the
current balance of the account. The method will return the amount withdrawn from the
account. If the transaction was unsuccessful, 0 will be returned
3) Method List (private):
▪ bool insert_pin() – Method that will be furtherly used in the interaction operations with the
account. This method will allow the user to insert a pin using the “cin” routine, up to 3 times. If
the pin was inserted 3 times wrong, False will be returned. If the pin was inserted correctly,
True will be returned.
4) Friend function:
▪ void transfer_money(Account &account_1, Account &Account_2, float u_amount) . This
method will transfer money from the first account, to the second account, by taking use of the
previously defined class members found_account and withdraw_money. The account 1 will
transfer the money to the second account.
5) Main function:
▪ Instantiate 1 Account class with balance 0
▪ Instantiate 1 Account class with balance 10000.
▪ Try to withdraw money from both the accounts and observe which withdrawal process was
successful.
▪ Found both the accounts with 1000.
▪ Transfer money from the second account, to the first account.
