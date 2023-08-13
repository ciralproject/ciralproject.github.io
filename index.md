---
layout: home
header:
  title: CIRAL
  text1: >
    <h3> Cross-Lingual Information Retrieval for African Languages </h3>
  text2: >
    <h2> @FIRE 2023 </h2>
  action: # action button is optional
    label: Call for Submissions
    url: "https://forms.gle/Rzw1yWoDHqGBXv8N7"


sections:
  - type: track-overview.html
    section_id: description
    background_style: bg-primary
    title: TRACK OVERVIEW
    text1: >
      As information on the web continually expands across different languages, Cross-lingual information retrieval (CLIR) systems which enable users search in one language and retrieve documents in another are becoming increasingly important. Research in CLIR for African languages is also growing, and these methods often require African CLIR test collections to adequately evaluate systems and expand research. Collections have been curated which either include some African languages or solely focus on African languages, however, these collections are mostly created via translation or synthetically and could be prone to bias and translation issues.

    text2: >
      The goal of the CIRAL track is promote the research and evaluation of CLIR for African languages. With the intent of curating a human-annotated test collection through a community shared task, our track entails retrieval between English and four African languages which are Hausa, Somali, Swahili and Yoruba. Given the low-resourced nature of African languages, this track also focuses on fostering CLIR research and evaluation in low-resource settings, and hence the development of retrieval systems that are well suited for such tasks.

    # actions:
    #   - title: Get Started!
    #     url: '#page-top'
    #     class: btn-light

  - type: participation.html
    # this section has always ID 'portfolio'
    section_id: participation
    background_style: bg-white-50
    title: PARTICIPATION
    items:
      - title: Task
        text: Track participants are tasked with developing retrieval systems that return <em>documents</em> in a specified African language when issued a query in English. Retrieval is done at the passage level, with queries formulated as natural language questions and passages relevant to a given query are those with answers to the question. More details on the training and tests sets are provided in the <a href="#datasets">Dataset</a> section.
        icon: bi-tools
      - title: Submission
        text: Each team is required to submit run files obtained from their retrieval systems in the 6 column standard TREC format. Submissions are expected to be 2 to 3 per language, but with a cap of 3. Participants with more than 3 submissions in any of the languages would have the top 3 selected based on ranking by the team. Run files can be submitted using this <a href="https://forms.gle/M1XJi39evHfibPMB9">form</a>
        icon: bi-send-check
        #url: '#'
      - title: Evaluation
        text: Evaluation is done by creating pools for each query and manually judging for the binary relevance of retrieved passages (pooling depth is <em>k = 20</em>). Using the provided judgements, the submitted run files are evaluated with the following standard retrieval metrics - Recall@100 and nDCG@20.
        icon: bi-graph-up
        #url: '#'
      - title: Working Notes
        text:  Each team is required to submit a working note detailing their proposed retrieval system and approach to the task. The required format for the working note is the <b>Single Coulmn CEUR format</b>, with a minimum of 5 pages. Submissions would be made to the track’s email at <a href="mailto:ciralproject23@gmail.com">ciralproject23@gmail.com</a>.
        icon: bi-file-earmark-pdf

  - type: datasets.html
    section_id: datasets
    #background_style: bg-info
    title: DATASET
    text1: >
      For each language, a static collection of passages extracted from news articles is provided. The training set comprises of the static collection, approximately 10 queries per language and some binary relevance judgements for each query. <b>The queries and qrels in the train set serve as samples to help analyze relevance, and explore approaches while using the qrels for evaluation.</b> The statistics of the collection is documented in the dataset repo, and can also be found in the table on the right.

      <p>The datasets would be made available in respective Hugging Face repos (<a href="https://huggingface.co/datasets/CIRAL/ciral-corpus">Corpus</a>, <a href="https://huggingface.co/datasets/CIRAL/ciral/tree/main">Queries and Jugdements</a>)  according to the release date for each set. Participants can request for access to the training and test sets.</p>
    table: >
      <table border="1">
      <thead>
      <th> </th>
      <th class="no-borders"># Train Queries</th>
      <th># Test Queries</th>
      <th># Passages</th>
      </thead>
      <tbody>
        <tr>
        <td><b>Hausa (hau)</b></td>
        <td>10</td>
        <td>TBA</td>
        <td>715,355</td>
        </tr>
        <tr>
        <td><b>Somali (som)</b></td>
        <td>10</td>
        <td>TBA</td>
        <td>1,015,567</td>
        </tr>
        <tr>
        <td><b>Swahili (swa)</b></td>
        <td>10</td>
        <td>TBA</td>
        <td>981,658</td>
        </tr>
        <tr>
        <td><b>Yoruba (yor)</b></td>
        <td>10</td>
        <td>TBA</td>
        <td>82,095</td>
        </tr>
      </tbody>
      </table>
    # services:
      # - title: Corpora
      #   text: For each language, a static collection of passages extracted from news articles is provided. The news articles are obtained from the indigenous websites 
      #   #icon: bi-rocket-takeoff
      # - title: Evaluation
      #   text: We update dependencies to keep things fresh.
      #   #icon: bi-activity
      # - title: Training Set
      #   text: For each language, the provided training set consists of a monolingual collection of passages, approximately 10 queries and a few (an average of 10) relevance judgments for each query. These relevance judgments would help participants with analysis as well as tune their prototype systems.
      #   #icon: bi-gem text-info
      #   #url: https://startbootstrap.com/
      # - title: Test Set
      #   text: You can use this theme as is, or you can make changes!
      #   #icon: bi-rocket-takeoff


      # - title: Made with Love
      #   text: You have to make your websites with love these days!
      #   icon: bi-heart-fill
      # - title: Other 1
      #   text: Some not-so long text here.
      #   icon: bi-emoji-heart-eyes
      # - title: Other 2
      #   text: Some not-so long text here.
      #   icon: bi-emoji-sunglasses-fill

  # - type: aside.html
  #   section_id: aside
  #   title: Free Download at Start Bootstrap!
  #   actions:
  #     - title: Download Now!
  #       url: https://startbootstrap.com/themes/creative/
  #       class: btn-light


  - type: timeline.html
    section_id: timeline
    title: BULLETINS
    background_image: url(../img/globe_image.jpg)
    items:
    - title: Track Timeline
      icon: bi-calendar-event
      table: >
        <table class="track-timeline">
        <tr>
          <th rowspan="2"><s>22nd May 2023</s></th>
          <th>Track Website opens</th>
        </tr>
        <tr>
          <th>Registration for Track Begins</th>
        </tr>
        <tr>
          <th><s>7th Jun 2023</s></th>
          <th>Training Data Released</th>
        </tr>
        <tr>
          <th><s>1st Aug</s> 21st Aug 2023</th>
          <th>Test Data Released</th>
        </tr>
        <tr>
          <th><s>30th Aug</s> 10th Sep 2023</th>
          <th>Run Submission Deadline</th>
        </tr>
        <tr>
          <th><s>10th Sep</s> 22nd Sep 2023</th>
          <th>Declaration of Results</th>
        </tr>
        <tr>
          <th>2nd Oct 2023</th>
          <th>Working Note Submission</th>
        </tr>
        <tr>
          <th>8th Oct 2023</th>
          <th>Review Notifications</th>
        </tr>
        <tr>
          <th>15th Oct 2023</th>
          <th>Final Version of Working Note</th>
        </tr>
        </table>
    - title: Announcements
      icon: bi-megaphone
      table: >
        <table class="announcement">
        <tr>
          <th class="announcement-list">Documentation: Baselines, <a href="https://github.com/ciralproject/ciral/blob/main/Guidelines/README.md">Starting with IR/CIRAL</a></th>
        </tr>
        <tr>
          <th class="announcement-list">Train queries and qrels released for Swahili and Somali <a href="https://huggingface.co/datasets/CIRAL/ciral/tree/main">here</a></th>
        </tr>
        <tr>
          <th class="announcement-list" style="color:#495057">Updated version of corpora available in Hugging Face <a href="https://huggingface.co/datasets/CIRAL/ciral-corpus">repo</a></th>
        </tr>
        <tr>
          <th class="announcement-list" style="color:#495057">Training data released for Hausa and Yoruba <a href="https://huggingface.co/datasets/CIRAL/ciral">here</a></th>
        </tr>
        <tr>
          <th class="announcement-list" style="color:#495057">Corpora available <a href="https://huggingface.co/datasets/CIRAL/ciral-corpus">here</a></th>
        </tr>
        </table>


  - type: organizers.html
    section_id: organizers
    title: Organizers
    #background_style: bg-info text-white
    members:
      - name: Mofetoluwa Adeyemi
        text: University of Waterloo
        image: assets/img/members/Mofe.png
        url: '#'
      - name: Akintunde Oladipo
        text: University of Waterloo
        image: assets/img/members/Tunde.jpeg
        url: '#'
      - name: Xinyu Crystina Zhang
        text: University of Waterloo
        image: assets/img/members/Crystina.png
        url: '#'
      - name: David Alfonso-Hermelo
        text: Huawei Noah's Ark Lab
        image: assets/img/members/David.png
        url: '#'
      - name: Jimmy Lin
        text: University of Waterloo
        image: assets/img/members/Jimmy.png
        url: '#'
      - name: Mehdi Rezagholizadeh
        text: Huawei Noah's Ark Lab
        image: assets/img/members/Mehdi.png
        url: '#'
      - name: Boxing Chen
        text: Huawei Noah's Ark Lab
        image: assets/img/members/boxing_chen2.png
        url: '#'

  # - type: contact.html
  #   section_id: contacts
  #   title: Contacts
  #   text: >-

    # actions:
    # - title: +1 (202) 555-014
    #   icon: bi-telephone-fill
    # - title: E-Mail
    #   icon: bi-envelope-fill
    #   url: mailto:contact@yourwebsite.com
    # - title: Twitter
    #   icon: bi-twitter
    #   url: '#'
    # - title: Facebook
    #   icon: bi-facebook
    #   url: '#'
---

