# comp6451-p0-assignment-2---ethereum-programming-solved
**TO GET THIS SOLUTION VISIT:** [COMP6451 P0 Assignment 2 – Ethereum Programming Solved](https://www.ankitcodinghub.com/product/unsw-comp6451-p0-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;124401&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP6451 P0 Assignment 2 – Ethereum Programming Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Assignment 2 – Ethereum Programming

(Distribution to third parties and/or placement on non-UNSW websites prohibited.)

Background

Assignment Project Exam HelpIt’s election year, and you have been commissioned to develop a blockchain

• In the first phase of counting, we determine the number of first preferences each candidate received. If any candidate was the first preference of more than 50% of voters, then they are the winner of the election. • If no candidate received more than 50%, we declare that the candidate with the least number of first preferences is a loser, and eliminate them from further consideration. The votes of voters who had that candidate as their first preference are then redistributed to the remaining candidates, using the second preferences of these votes.

• This process repeats until some candidate has more than 50% of the vote. (In case of a tie, the election will be repeated between just the two remaining candidates. It is not necessary for you to implement this repeated election.)

Some further requirements for the election are the following:

• Only properly registered voters should be able to vote.

• Since election campaigns can be expensive to run, and operating an election also imposes costs on the election authority, voters are required to pay a voting tax when they vote. The amount of the voting tax is set by

Assignment Project Exam Helpthe election authority. After the election, 50% of the voting tax collected

from a voter is paid to that voters most preferred candidate as a contribution to the cost of their campaign. The other 50% is paid to the election authority to cover the costs of the election.

are several types of actors in this system:

• An election authority, responsible for ensuring correct operation of the election.

• Candidates

• Voters

Assignment Project Exam Helpdoes not reveal the actual vote, but commits the voter to an actual vote.

amount is attached. Any amount greater than the voting tax should be repaid to the voter.)

vote cast by a voter will count; earlier votes will be discarded. The voting tax needs to be paid only for the first vote.

• A voters actual vote should be a list of numbers that orders the set of all candidate numbers {1,…,n} in some way. For example, if n = 3 then [1,2,3] and [3,1,2] are valid votes. A list of numbers is not valid if it does not contain all the numbers 1…n, if it contains any other numbers, or if it contains repeated numbers.

• The implementation should provide some way by which candidates and the election authority receive their share of the voting taxes collected.

Assignment Project Exam Helpsatisfied.

voters, This means that the election authority is responsible for deciding who is an eligible voter, and (because voters are anonymous in the system) making sure that no voter is registered more than once. (Double voting is not allowed.)

Suppose that this power has been delegated to registration authorities. Rather than operating on the blockchain, these authorities issue cryptographically signed certificates stating that a particular address belongs to an eligible voter. Specifically, the certificate should be a message (effectively) stating

I, authority-address assert that address voter-address is controlled by a voter who is eligible to vote in the election, and no other address controlled by this voter is currently registered.

The system should accept such a certificate as sufficient evidence that the voter is eligible for registration, provided it knows that the authority-address belongs to an approved registration authority, and the message is correctly cryptographically signed by this authority.

Implement this idea by adding the following functions to your solution from part 1.

• register certified voter(voter-address,authority-address,certificate):

Deliverables

Assignment Project Exam HelpSubmit the following. Note that it is not a requirement of the assignment to

develop a Graphical User Interface for this application – where code other than Solidity code is necessary, invocation using command line instructions suffices to meet the requirements.

tion of the overall system. The report should

• In case use of the smart contract requires off-chain computations not implemented in the smart contract, explain what this code does and how to compile and/or operate it. You are not required in this assignment to develop a fancy user interface for any such code: some simple command-line scripts suffice.

• For each of the requirements above, briefly indicate where and how your code meets the requirement. Briefly explain each of the functions in your code. In case you identified any missing requirements or specification ambiguities in the course of your analysis of the application, state what these are and what you have done to resolve and implement them.

• Provide an analysis of the running costs in gas and Australian dollars of the application from the point of view of the candidates, voters and election authority, and how this depends on factors such as the total number of candidates and voters. Take into account current information on the costs of transactions on the Ethereum public blockchain, and the gas costs of running your code.

• Describe any security considerations concerning the system and its operation that you consider should be pointed out to the (various classes of) users. Are there any specific traps that the user needs to avoid in using the system, and if so, what are strategies that the user can apply to avoid these traps. • Explain how your code avoids common Solidity security vulnerabilities like reentrancy attacks.

• Reflectively discuss the overall suitability of the Ethereum platform for this application.

Proper acknowledgement of any sources of information or libraries you have used in your project is required.

If you have used any public Javascript libraries, to avoid an overly large

Assignment Project Exam Helpsubmission file, do not include these, but ensure that there is sufficient

information in your submission that these can be automatically installed. In particular, include your package-lock.json file.

command line arguments are required to run your tests, include a script that allows the appropriate calls to be made easily by the marker. In any case, the report should contain all the information that is required to determine how to run your tests.

Resources and Hints for Testing

For Part 1, it will probably be possible to write tests for your code entirely using test scripts written in Solidity. Part 2 is more challenging, since it requires constructing ECDSA signatures, for which Solidity does not provide good support. (The built-in function ecrecover only does signature verification.) For this, it is better to write tests in Javascript. In general, JavaScript testing is the more powerful approach (better supported because off-chain application code for interacting with the Ethereum blockchain is most commonly written in JavaScript) and there are a number of JavaScript libraries that support testing.

• Truffle Documentation https://trufflesuite.com/docs/truffle/. See, in particular, the section “Debug and Test”.

• The truffle-assertions library https://www.npmjs.com/package/truffle-assertions

• Ganache time-traveller https://www.npmjs.com/package/ganache-time-traveler helps to test

Assignment Project Exam Helptime-based properties.

Submission

from your CSE account using the command give cs6451 assignment2 &lt;tarfile&gt; on a CSE server.
