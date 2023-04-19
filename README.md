# Voting-System_C
Mini voting system

This is a C program that implements a mini voting system. Here are the main components of the program:


A struct called currentValidID which stores the current valid user ID parameters.
A struct called CANDIDATE which stores information about a candidate such as their candidate ID, name and number of votes.
A global array called candidateArray which stores information about all the candidates.
A variable called numberOfCandidates which stores the total number of candidates standing for the election.
A global array called studentVotes which stores information about the votes given by each student.
The program includes the following functions:

extractYear(char userID[15]) - this function extracts the year from a user ID. For example, if the user ID is 2018btecs00064, the function returns 2018.
extractRollNo(char userID[15]) - this function extracts the roll number from a user ID. For example, if the user ID is 2018btecs00064, the function returns 64.
checkBranchCode(char userID[15]) - this function checks whether the global branch code and inputed branch code is matching or not.
authenticateAdmin() - this function prompts the user for an admin username and password and checks if they match the predefined values.
banID() - this function creates a file called Banned.txt which contains the roll numbers of students who have been banned from voting. The user enters the roll numbers to be banned one by one until they enter 0.
createCandidateFiles() - this function creates a text file for each candidate containing their candidate ID, name and number of votes. The files are named candidate1.txt, candidate2.txt, etc.
deleteIllegalVote(char userID[15]) - this function deletes an illegal vote (i.e., a vote that was cast by a banned student or a vote that was cast for a non-existent candidate). The function takes the user ID of the student whose vote is to be deleted as an argument.
getWinner() - this function determines the winner of the election. If there is a clear winner, the function returns their candidate ID. If there is a tie or if no candidate has more votes than the others, the function returns -1.
initiateNewElection() - this function initializes a new election. It prompts the user for the year, branch code and total number of candidates standing for the election. It also prompts the user to enter the candidate IDs, names and number of votes for each candidate.

Overall, this program provides basic functionality for a voting system, including user authentication, vote counting and winner determination.
