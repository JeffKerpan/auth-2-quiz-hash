# Storing Passwords Quiz
## Would you like salt with your hash?


With your partner, in words both of you will understand 6 months from now, answer the following questions.

> A customer hires you to consult on a web app.  You notice that they are storing their passwords in plaintext.  What advice would you give the customer.  This advice should outline the risks of the current solution, and give a list of best practices for a new solution.

1st of all, NEVER EVER store your passwords in plaintext form. This is
extremely susceptible to being found by someone and used for ill will. Someone
would not even have to hack your information to get your passwords. Avoid
storing passwords if you do not need to. If you absolutely have to store a
password, use the hash and salted method. This encrypts your
 passwords making them much harder to hack into. Using both hashing and salting
adds extra layers of protection.    

> You are tasked for creating a RFP (request for proposal) for a new cryptographic hashing algorithm.  What requirements would you put in place for this new algorithm.

The hashing algorithm should be quick and easy. The hashes should always be the
same size regardless of the size of the text being hashed. You never want
collisions (2 different strings that create the same hash). You never want 2
similar strings to produce the same hash. By salting the hashes(adding a random
string to the password before creating the hash) you are adding) you are adding
that extra layer of protection that will make cracking the passwords take that
much longer. Although it should be quick enough to create a single hash,
creating thousands of hashes should take long enough to deter hackers.
