# Secret-Santa-BackTracking
This Code solves the problem of picking a unique secret santa partner in a group of 16 people that they have not had in a previous year. The data of all previous years is stored in a matrix. Each person is numbered 0
through 15, and the matrix index [i][j] has a value from 0 to 15. This represents the year that person i had person j. A -1 is used to represent uninitilazed years. Every number, representing the year, appears only once in each column and row. The goal of the program is to find a solution such that every participant has a partner that they have not previously had, and that each person is picked only once. The matrix represents data from the last 5 years, and the code generates solutions up to the 14th year. This is because multiple participants did not participate in every year of secret santa, this means on the last year, multiple people's only partner will be the same person, one of the participants that was not present all years. Without a backtracking approach, it is possible to pick partners from the sets of each members possible partners such that it is impossible to complete the current year of secret santa, because all of the possible partners of the remaining members could be used. The backtracking approach ensures that we find a solution each time the code is executed, and when we want to save the current state of the matrix to use for the next year, there is a cell that saves the matrix to a new text file. Sensitive data such as passwords and email addresses have been left out for privacy reasons.
