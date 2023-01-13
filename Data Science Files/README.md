TABLE OF CONTENTS:

Accessibility_Success_LogReg.ipynb:
    This file containtains a jupyter notebook script which will import the
    file below (Success_of_Accessibility_Initiatives.csv), conduct some
    simple exploratory data analysis and cleaning, create a logistic regression, test the regression for accuracy, and create a confusion matrix.

Success_of_Accessibility_Initiatives.csv
    This file contains columns and rows corresponding to a number of projects
    The columns are as follows:
        Business_Name: A string containing the name of the business
        Initiative_Name: A string containing an abbreviation of the project or initiative in question.
        Date: The date of the press release, product launch, or other initiative announcement.
        Consumer driven: A binary variable where:
            1 -> The project/initiative is consumer facing
            0 -> The project/initiative is not consumer facing
        Autism: a binary variable where:
            1 -> The project/initiative is catered towards inclusion of people with autism
            0 -> The project does not directly seek inclusion for people with autism.
        Aging: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of elderly people
            0 -> The project does not directly seek inclusion for elderly people.
        Deaf: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of deaf people
            0 -> The project does not directly seek inclusion for deaf people.
        Blind: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of blind people
            0 -> The project does not directly seek inclusion for blind people.
        Speach: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of  people with speech impediments
            0 -> The project does not directly seek inclusion for people with speech impediments.
        Light Sense: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of light-sensitive people.
            0 -> The project does not directly seek inclusion for light-sensitive people.
        Wheelchair: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of people without four fully functional limbs.
            0 -> The project does not directly seek inclusion for people without four fully functional limbs.
        ADHD: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of people with ADHD.
            0 -> The project does not directly seek inclusion for people with ADHD.
        Mental_Health: A binary variable where:
            1 -> The project/initiative is catered towards inclusion of people with mental health challenges.
            0 -> The project does not directly seek inclusion for people with mental health challenges.
        Company_Code: A binary variable where:
            A string containing the symbols which the country trades under on the stock market
        Initiative_Close:
            The evaluation of the company's stock on the day of the initiative/project
        Month_Close:
            The evaluation of the company's stock one month after the day of the initiative/project
        Success: A binary variable where:
            1 -> The stock gained value over the course of the month
            0 -> The stock lost value / remained the same over the course of the month
    In the creation of this project, I relied upon the information at these websites:
        -https://aboutamazon.com/news/devices/meet-amazon-employees-making-alexa-more-accessible
        -https://blogs.microsoft.com/blog/2021/04/28/doubling-down-on-accessibility-microsofts-next-steps-to-expand-accessibility-in-technology-the-workforce-and-workplace/
        -https://www.apple.com/newsroom/2022/05/apple-previews-innovative-accessibility-features/
        -https://www.blog.google/outreach-initiatives/accessibility/wheelchair-users-google-maps/
        -https://www.accenture.com/hu-en/case-studies/about/accessibility-every-moment
        -https://www.verizon.com/about/news/verizon-launches-disability-advisory-board
        -https://www.vercida.com/uk/articles/disability-allyship-at-meta
        -https://www.businessinsider.com/guides/tech/what-is-uber-assist
        -https://learning.linkedin.com/content/dam/me/learning/en-us/pdfs/new_dei_content.pdf
        -https://digitability.com/ibm/
        -https://www.youtube.com/watch?v=CrB8Hf7FReU&t=19s
        -https://www.bhp.com/news/articles/2019/08/neurodiversity-through-our-teams-eyes
        -https://www.hcamag.com/us/specialization/diversity-inclusion/dell-manager-how-tech-giant-recruits-and-supports-neurodivergent-talent/405669
        -https://cloud.google.com/blog/topics/inside-google-cloud/google-cloud-launches-a-career-program-for-people-with-autism
        -https://www.hpe.com/us/en/insights/articles/designing-a-hiring-practice-for-autistic-it-staff-1812.html
        -https://blog.adobe.com/en/publish/2022/10/05/celebrating-neurodiversity-in-the-workplace
        -https://www.techrepublic.com/article/amazon-alexa-the-smart-persons-guide/
        -https://www.technology.pitt.edu/content/live-transcription-zoom-arrives-february-12-requires-host-activation#:~:text=Live%20Transcription%20for%20Zoom%20Arrives%20February%2012%3B%20Requires%20Host%20Activation,-Friday%2C%20February%205&text=Zoom%20Videoconferencing%20will%20enable%20automatic,bottom%20of%20the%20meeting%20video.
        -https://www.audioeye.com/post/wcag-3-future-accessibility-standards/
        -https://www.apple.com/ca/newsroom/2022/05/apple-previews-innovative-accessibility-features/




