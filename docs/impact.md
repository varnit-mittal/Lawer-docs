# Feedback
<ol>
<li>
<p>
<b>Issue:</b>  Limited Accessibility of Precedent Search for Laypersons
</p>
<p>
<b>Description:</b> Traditional keyword-based precedent search methods relied heavily on legal jargon, posing a significant barrier for those without specialized training.
</p>
<p>
<b>Resolution:</b>  Inspired by user feedback, the team undertook the following steps:
<ul>
<li><b>Solution Concept:</b> Develop a situation-based precedent search function to enhance accessibility.</li>
<li><b>AI Implementation:</b> Integrate Gemini AI to enable natural language processing, allowing users to describe their legal situations in plain terms.</li>
</ul>
</p>
<p>
<b>Impact</b><br>
<ul>
<li><b>Improved User Experience:</b> Laypersons can intuitively find relevant precedents without specialized knowledge, leading to a smoother and more empowering experience.<br></li>
<li><b>Increased Accessibility:</b> The application becomes a valuable resource for a wider audience, bridging the gap between legal knowledge and everyday understanding.</li>
</ul>
</p>
</li>

<li>
<p>
<b>Issue:</b> Incorrect Category Mapping Due to Suboptimal Gemini Model Parameters
</p>
<p>
<b>Description:</b> Initial parameter settings for the Gemini model resulted in the misclassification of items within certain categories. This error was not detected during the internal development and testing phases.
</p>
<b>Resolution:</b>  Following user feedback highlighting the misclassifications, the team conducted a thorough analysis.  Key parameters, such as temperature, were adjusted to optimize the Gemini model's performance.
<p>
<b>Impact</b><br>
<ul>
<li><b>Improved Accuracy:</b> Parameter optimization significantly enhanced the accuracy of category mapping, ensuring correct classifications within the system.</li>
<li><b>Enhanced User Experience:</b> The correction of mapping errors streamlined the user experience, eliminating confusion and frustration caused by incorrect classifications.</li>
</ul>
</p>
</li>
</ol>
<p>Users were delighted about the new searching capabilities of our application and lawer did not let down. We had users test out search based upon different types of criminal situations and lawer provided them relevant legal precedants. </p>

# Scalability

Lawer currently operates upon Indian law database with the api of the [indiankanoon.org](https://indiankanoon.org/). This application has a huge scalability and our team is soon gonna start on some of them. Some possible extensions are:- 
<ul>

<li>
Extension towards the legal databases of other nations, this sort of extension would require access to the the central judicial databases of other nations. 
</li>
<li>Multi language support, this will promote inclusivity and help lawer reach a larger audience. This extension will be easily achievable with the help of <a href="https://cloud.google.com/translate/docs/reference/rest">cloud translation api</a>.</li>
<li>
Multi platform support. The application is currently supported on android only, our team aims to provide multiplatform support like ios and web. Flutter's multiplatform supprt will be a huge help in this, with a little restructuring of files and referencing the documentation, we will soon make lawer available on every screen
</li>
</ul>
The scalability factors mentioned above focus more on increasing the audience base, our team have planned many other extensions making the application more functionality rich. Some of these ideas are 
<ul>
<li>
<b>Law of the week:</b> We want to empower our users by providing easy-to-understand explanations of laws that affect their everyday lives. This extension will promote engagement to our application and legal awarenes of the general public will increase. 
</li>
<li>
<b>AI legal assistant: </b>It often happens that civilians are stuck in situations where approaching a legal advisor is difficult. Our AI legal assistant would be just what the user needs in such a situation. We can use the gemini AI model for this functionality, with the amazing natural laguage processing of the model, we can get this ready. With some training, our AI model can provide the legally correct sequence of actions for an individual, this will be a handy tool for many.
</li>
</ul>