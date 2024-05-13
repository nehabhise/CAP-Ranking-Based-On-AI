# CAP-Ranking-Based-On-AI
For running this application we need python installed and should have firebase db. Any editor for opening html, js files will work.

Conducting a good recruitment process and selection process is majorly important for an organization. The main purpose of the paper is to analyse how the system will work and will be effective for recruitment. The paper considers modern technologies, algorithms, and selection strategies of an organization for the recruitment process. Finding indicates that this recruitment system reworks the traditional recruitment process into a time and space independent, synergetic hiring process. In this paper, we have suggested a system which will help the Human Resources to shortlist specific candidates whoever are suitable for the position which HR is looking for. The system is based on CV ranking, aptitude test and psychometric test. By using this system workload of HR and time to shortlist the candidate will reduce to a certain extent. Test scores with CV scores and HR analysis strategies are considered for shortlisting a good candidate. Thus, by using this system for candidate’s selection, fair decision will be taken. Weighted Majority Voting Algorithms are used for generating ranks and shortlisting purposes.

Algorithms and Techniques:
Weighted Majority Voting Algorithm :
▪ It gives some votes different amount of weight concerning the outcome of an election.
▪ Each individual is called player and these players have been given some weight.
▪ Quota is minimum weight needed for vote to pass need. q:w1,w2,w3,…wn where q is quota and w1,w2,w3,etc are weights.
▪ Player having weight equal to or greater than quota is dictator. Ex:[20:21,6,3]
▪ If a vote is never essential for a group to reach quota then that is called as dummy.
Ex: [16:12,10,2]
▪ If the support of any player necessary for the quota to be reached its Veto power. Ex:[30:19,15,11]
Design Algorithm:
For CV analysis we used the machine learning algorithm (TF-IDF). In our system, this algorithm is used for extracting the more accurate keywords from the CV. TF-IDF algorithm is most widely used text mining algorithm.
Its working is mentioned below:

Step 1: Calculate Term Frequency i.e.TF

TF – It is used for calculating the number of times that particular keyword is found in that CV / total count of keywords appeared in CV.
TF (‘keyword1’) =number of times ‘keyword1’ appears in CV /Total number of keywords in the CV. Here, the term “keyword1” specifies any job specific skill requirement specified by the HR for which algorithm is working.

Step 2: Calculate Inverse Document Frequency i.e. IDF

There is a chance of appearing less required keyword. So, to overcome this problem IDF is used.
IDF checks the log value = 1 for the required CV as per job skill and log value = 0 for the unwanted CV.
IDF (‘keyword1’) = log (total number of CV/Number of CV with term ‘keyword’)

Step 3: Calculate TF - IDF score

score= TF (‘keyword1’) * IDF (‘keyword1’)
As the score increases, more relevant that CV is and chances for candidate selection is increased. In this test applications are reduced as irrelevant CV’s are discarded. This step is used for classification to separate out the relevant and irrelevant CV as per score.

Step 4: If candidate is selected on the basis of CV, then HR will call the candidate in company’s premises for giving aptitude and psychometric test. Separate link will be provided to their email ids and ask for them to give test.

Step 5: Aptitude and psychometric test score are calculated. And the Weighted Majority Voting Algorithm is applied to find the rank.






