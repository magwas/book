## Communication

As we have seen, communication is the key. The challenge is to provide relevant, high quality information within the comprehension of the individual, where this ability itself vary widely among people. The relevance requirement also means that everyone should have a reasonable opportunity to participate in the communication, whereas the quality requirement means that offtopic or even just excessive amount of information should not be allowed. Well, these are conflicting requirements.

The good news is that in ideal sized groups we can count on our naturally evolved skills to come up with a reasonably good balance.

In metagroups, the official communication is made by the officials and issue representatives of the metagroup, and as a result of the formal decision-making procedure of a node directly below. A form of communication is a non-binding vote, where the one communicating is free to name the alternatives, but the dummy alternative must present.

Informal nodes owned by formal nodes must work transparently, all financial transactions and all documents which do no contain sensitive data are being public and searchable by all individuals having the same eligibility as the eligibility requirements of the owner node. This rule is recursive: nodes under or owned by owned nodes should also adhere to it.

Representatives are expected to have over the average communication and negotiation skills, as they are selected to the task by people based exactly on these skills.

The approach to formal communication is that it is categorised based on the initiator and the properties of the issue at hand, and each individual can select which categories they choose to receive on which device. There is of course also a choice of what to actually overview. Categories could include

* notifications about different phases of the decision making process in nodes \(a notable example being decision making process initiation directly in a metagroup by an individual\),

* all or topic-specific official communication of nodes or representatives,

* communications related to a specific decision-making process,

* messages from individuals, further subdivided based on friendship or membership

* financial transactions filtered on initiating and receiving entity and amount

* documents issued by owned nodes, filtered by office and type

* for representatives based on whether the individual is represented, and whether it actually delegates the representative

The above formal communication is augmented with the ability to comment every information in the system, including proposals, alternatives, financial transactions and documents. Comments are organised in threads and can only be deleted by the commenter, but can be up- and downvoted and flagged by different aspects \(like offtopic, inadequate language, etc\), and individuals can choose which comments to show and how, based on this information.

All of the information in the system \(down to individual comments\) can be cross-referenced.


### The communication subsystem as a social media platform

As the communication system allows everyone to create and comment on messages, it is essentially a social media platform in itself.

## Goals as a social media platform

A social media platform should be *conductive to civilized, fact-based discussion, which leads to good decisions and concerted actions*.

A subset of the problem can be viewed as avoiding the known shortcomings of current social media platforms:

* fake news
* extremisms and the related inability to engage in productive discussion
* filter bubbles

The problems with current social media platforms can be tracked down mostly to the following phenomenon:

* the incentives provided to users are not conductive to the goals of an ideal social media platforms
* the filtering algorithms are tuned in a way which optimizes for engagement and against civilized discourse
* the moderation is too heavily leaning on algorithmical solutions, which are unable to adequately decide on moderation related questions


#### Community moderation experiments

Regarding the last point, there are a couple of more or less successful experiments on community moderation. One such example is the forums and article comment areas of [Ars Technica](https://arstechnica.com/civis/).
That system allows users to "upvote" and "downvote" comments, while the user should choose the reason of the feedback from a small set of reasons (agree, interesting, adds to story, disagree, inaccurate, doesn't contribute, abusive).
The system automatically hides comments with too low score. Those comments can be still read, but it needs additional action in part of the reader, so offtopic and abusive comments are effectively filtered out without inproportionately affecting free speech.

It successfully solved the following challenges:
* high quality of content: it is repeatedly pointed out that some of the comments add significant information and analysis to the article. Those comments also have high visibility.
* civilized discourse and troll resistance (due to filtering out abusive and offtopic content)

The Ars technica approach is not ideal though (as it can be argued that the problem itself is only asymptotically solvable): there are policy issues on which the user community have a more or less established view. There are cases when otherwise factual or civilized comments are downwoted because they are either dissenting with the prevailing world view or viewed as dissenting because they intend to fix minor errors or omissions on a comment communicating the prevailing world view.

The source of this is arguably the fact that subjective aspects (based on choice of values) and objective ones (regarding factuality and adherence to moderation policies) are mixed. Because that kind of bias is one of the most fundamental limits of effective decision making, it is important to positively incentivize factual and civilized dissent, and make every (automated and human) agents of the systems learn from moderation mistakes related to them.

Another good example of working community moderation is [Stack Overflow](https://stackoverflow.com/). The goal behind moderation and scoring there is direct useability of the answers. As this is a much more narrow goal than that of a generic social media site, they could reach very good results with a relatively simple scoring system, using reputation points. An interesting aspect of the system is that they use the reputation points to enable functions aimed at quality control.

#### Incentive and moderation model for social media

The main idea is that users have a set of points (e.g. experience, wisdom, tolerance ...), with which they can build their online characters similarly to role playing games.

Messages can be up- and downvoted with giving the reason. There are two broad sets of reasons: subjective and objective. Those two sets are clearly separated, thus helping to make the distinction between the two categories.

Feedbacks (up- and downwotes, comments) result in changes for points for both the user doing and receiving the feedback. The rules related to points should be designed in a way which incentivizes users towards the goals defined above.

#### Scoring and moderation rules

As the exact set of rules should be the result of fine-tuning, all rules mentioned below should be viewed only as suggestions, subject to moderation policies decided by the community. As all rules in the system, higher levels should have broader sets of rules which are concretized in lower levels. This provides a diversity which in the social level allows for cultural differences, and in the technical level allows paralell experimentation with different sets of rules, hopefully resulting faster convergence towards an optimal ruleset based on experience.

Low points for objective criteria of a message results in moderation, which normally means hiding the message (changing the message to a statement about how it is problematic, and adding a control which makes it possible to view the message nevertheless), and in extreme cases results in deleting the message altogether. A poster of a message have the chance to amend the message to alleviate objective concerns related to it. In this case the users given the negative feedback are expected to revise their verdict. Official communications are never hidden, but still marked with a prominent warning.

Downvotes for objective aspects should mark the part of the message deemed as problematic, and explain exactly how are they problematic (which part of the moderation policy is violated, and any related established facts). Objective downvotes can ask for moderation decision, as the author of downvoted message can also do so. First round of moderation can be algorithmic, and any moderation decisions can be appealed. Moderation appeals follow the rules of conflict resolution. Moderation decisions also affect the points received by the poster and users giving feedback; e.g. if the decision finds out that the moderation rules were violated, upvoters with the related reason(s) got their wisdom points reduced, downvoters get it increased, while in the opposite case the opposite happens.

Some possible scoring rules:
* Any feedback results in increase of experience points
* Negative feedback on subjective aspect and simultaneous positive feedback on objective aspect result in increae of tolerance point.
* Poisitve feedback on objective aspect and negative feedback on objective aspect results in increase of wisdom point.
* The two above results can be changed based on actual moderation decision.
* Subjective feedbacks can also increase/decrease points, e.g. increase tolerance for show of tolerant behaviour, increase courage for brave behaviour, increase funnyness for funny remarks.
* If revising a statement with negative objective feedback results in revising the feedback, that worths wisdom points.
* Failure to revise feedback for a revised statement results in decrease of tolerance.
* Given that some of the messages are official communications of groups or offices, it is technically possible to use scoring rules for them. It is an open question whether (or in which cases, along which rules) it is a good idea.

#### Hero labels

Outstanding real-world actions can be awarded with hero labels. Hero labels can be awarded by a group, based on voting. The receiver of the label can choose whether to display it in its main profile page (but all the labels can be queried for a given user, including nondisplayed ones). A legitimate use of hero labels is to award labels with negative connotations to players who are viewed to play a negative role in some important issue.


#### The role of algorithms and AI

As we have seen, the problems of current social media platforms are partly traceable back to inadequacies of algorithms used. The reason for using algorithms is to reduce the human resource needs for filtering and moderations. This is a legitimate use, which no social media above a given traffic can avoid. However ultimately trusting decisions on algorithms denies the complexity of social interactions and - as we have already seen wrt. Brexit and the election of Donald Trump - can have very serious consequences. Therefore algorithms should only used as the first line of defence in moderation, and care should be taken that decisions overriding algorithmic decisions are used to train the algorithms.

The use of algorithms for filtering is an even more complex problem.


It is arguable - and one of the main arguments against current social media - that enforcing one algorithm for everyone gives disproportionate power to the one controlling the algorithm: not just because the decisions are trusted in a single agent, but also because the information those decisions are based on are highly personal information. Fortunately today's computing resources make it possible to do such filtering on personal devices, trained by the end-user and personal information kept on the device. This should be the primary modus operandi.

Using personally trained filtering does not solve all problems, and makes solving some problems harder. A fundamental problem is balance between engagement and civilized discourse. As an algorithms offers more and more engaging messages, it more and more distorts the view of the user on reality, making discourses more and more subjective, losing focus and hence being unconductive from a decision-making perspective. Conversely, an algorithm which shows a balanced selection of messages, more probably selects messages which are not emotionally engaging, or messages with a world view conflicting that of the user, with which they cannot easily relate to - and less easily relate to in a socially acceptable manner. We call this pheomenon "the inconvenient thruth".

Our system tries to put emphasis on incentives about dealing with inconvenient thruth in a manner which in turn makes it easier for others to deal with the messages. The motivation is not about reading messages which good to read, but about dealing with them in the "right" way. This in itself does not help avoiding filter bubbles; it merely helps to keep engagement once filter bubbles are eliminated.

In current systems, ultimately the user is the one who trains the algorithms. In case of current social media it is done in a less straightforward manner, by liking and replying to posts. This can be made more straightforward, by making the training a set of explicit decisions. For some users, this could help keeping the bubble wider, by consciously including messages from players with differing world views, as some users consciously "like" players who have diametrically opposed views just to keep their bubble more open. However in the general case it depends on user behaviour, because currently used algorithms cannot distinguish between topics and sentiments. For example such an algorithm puts fans of a soccer club into one bubble, and fans of its rival club in another bubble. An algorithm which filters on topic, and not sentiment, would put members of both fanbase to the same bubble. When we are designing a system for decisionmaking, this is the right behaviour: bothering the user with uninteresting topics is contraproductive, while giving all views on a given topic helps to make better decisions. Unfortunately this topic is highly technical, and the current state of the art does seem to put it to the set of unsolved problems. A possible - more slowly converging - solution is to measure how often a user engages in discourse with people of different world views, and use the scoring system to reflect that. It seems to be a problem which can be more easily tackled than filtering algorithms for topic and not sentiment. This in turn would provide incentive for users to choose better algorithms and train them in a more open manner, which in turn would incentivize algorithm developers to put more efforts to such algorithms.



