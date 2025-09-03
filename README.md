ObjectIves:

A) Calculate sample average, sample standard deviation, and standard error of the sample mean of the sample size of polls in this dataset. To determine a useful measure of poll accuracy. Found absolute delta between poll margin and actual margin, or absolute error.

B) Generate 12 random subsamples from the dataset, each containing 20 polls. Determining how much does the average accuracy of these 20 polls varies from subsample to subsample? Is this consistent with whole dataset?

C) Determine whether polling accuracy has been growing or not over time: (i) overall; (ii) consider alternate units of measurement between race types.

D) Determine if large samples are really necessary for poll accuracy. Is there even a correlation between sample size and the fact that a poll gets the winner right?



Categorical Column Data Descriptions:

poll_id
FiveThirtyEight poll ID number.

question_id
FiveThirtyEight question ID number. Note that there may be more than one question from the same poll included in the data.

race_id
FiveThirtyEight race ID number.

cycle
Election cycle.

location
Geography of the question. This may be a state, House district, or the US.

type_simple
Category of the race. This value is structured with the type of election (Sen, Gov,Pres, or House) followed by a dash, and then either P or G to indicate if the survey is of a primary or general election, respectively. House generic ballot polls are noted as House-G-US.

race
Race for this question. This is structured as the year, followed by an underscore and the simple type, followed by an underscore and the location. For presidential primaries, the party is indicated with a -R or -D after Pres.

pollster
Pollster name.

pollster_rating_id
FiveThirtyEight pollster rating ID number.

aapor_roper
Boolean flag for whether the pollster is a member of the AAPOR Transparency Initiative or contributes polls to the Roper Center.

inactive
Boolean flag for whether the pollster appears to still be conducting publicly available opinion polls.

methodology
Mode used to conduct this poll. This should be a combination of one or more of the following values, separated by a forward slash:

Live Phone — Live telephone interviews, may or may not include calls to cellphones

IVR — Interactive Voice Response, otherwise known as automated polls or "robopolls"

Online Panel — Opt-in online panel, either proprietary or contracted to a panel provider

Text-to-Web — Recruitment via text messages that direct participants to a website to complete the survey

Probability Panel — Probability based online panel

Email — Recruitment via emails that direct participants to a website to complete the survey

Mail-to-Web — Recruitment via snail mail that directs participants to a website to complete the survey

Mail-to-Phone — Recruitment via snail mail that directs participants to call a phone number to complete the survey

Text — Recruitment via text message in which questions are asked directly over SMS

Mail— By U.S. mail or other “snail mail” service

Online Ad — Recruitment via advertisement on websites, mobile games, or other online medium

App Panel — Opt-in panel using a proprietary app

Face-to-face — Poll conducted in person

partisan
Flag for internal/partisan poll. "D" indicates Democratic poll, "R" indicates Republican poll, "I" indicates poll put out by independent candidate's campaign.

polldate
Median field date of the poll.

electiondate
Date of the election.

time_to_election
Number of days between the median field date of the poll and the election date.

samplesize
Sample size of the question. For questions with no sample size available, this is approximated as the median sample size for races of the same type.

cand1_name
Name of Candidate #1. Candidates #1 and #2 are defined as the top two finishers in the election (regardless of whether or not they were the top two candidates in the poll). In races where a Democrat and a Republican were the top two finishers, Candidate #1 is the Democrat.

cand1_id
FiveThirtyEight ID number for Candidate #1.

cand1_party
Party code for Candidate #1.

cand1_pct
Candidate #1's share of the vote in the poll.

cand1_actual
Actual share of vote for Candidate #1

cand2_name
Name of Candidate #2.

cand2_id
FiveThirtyEight ID number for Candidate #2.

cand2_party
Party of Candidate #2.

cand2_pct
Candidate #2's share of the vote in the poll.

cand2_actual
Actual share of vote for Candidate #2

margin_poll
Projected margin of victory (defeat) for Candidate #1. This is calculated as cand1_pct - cand2_pct. In races between a Democrat and a Republican, positive values indicate a Democratic lead; negative values a Republican lead.

margin_actual
Actual margin in the election. This is calculated as cand1_actual - cand2_actual. In races between a Democrat and a Republican, positive values indicate a Democratic win; negative values a Republican win.



