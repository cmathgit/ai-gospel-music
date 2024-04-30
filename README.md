# ai-gospel-music

# Using AI to generate biblically accurate gospel songs, among other genres, and music videos. Various Python scripts to auto generate prompts for Suno API and integration with Chat-GPT, YouTube, and more.

# Using AI to generate instrumentals for vocalists from a variety of genres, musical keys, and modes.

# Python script to send an API request to generate songs via SUNO AI, save the API response JSON format, read that data, parse the JSON array to get the information that we need, and write that information to execute more api requests or to a text file for logging. 

# Utilizes dictionaries of instruments, books of the bible, musical keys and modes, and vocalists of varying ranges and types to randomaly generate prompts for Suno AI requests.

# Bible Gateway can be implemented to pull the verse of the day for generating lyrics. For the King James Version, use this url
```
https://www.biblegateway.com/votd/get/?format=JSON&version=9
```
# Sample code to call the Biblegateway API URI for the Verse of the Day
```
    #Use Bible Gateway Verse of the Day
    votds = get_bible_votd_kjv()
    print("Bible Verse Content: ", votds['votd']['content'])
    print("Bible Verse reference: ", votds['votd']['reference'])
    print("Bible Verse reference: ", votds['votd']['version'])
    biblecontent = votds['votd']['content']
    biblereference = votds['votd']['reference']
    bibleversion = votds['votd']['version']
```

# Requirements
```
Python3+
```

# install Python in Windows visit
```
https://docs.python.org/3/using/windows.html
```

# Check that Python is installed
```
Open CMD and type python.
If it exists, to see where this executable lives, type where python
If not, follow the instructions for installation at python.org
```

# How to compile and run in Windows (back slash)
```
python generate_biblical_lyrics_simple_prompts.py
```

# Suno AI Prompt Max Lengths

# Custom Generate Lyrics Prompt Max Length: 399
```
zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz
```
# try using length of 229
```
Generate passionate, meaningful, heartfelt, and profound lyrics to a full song inspired by and devoted to preserving the message of Song of Solomon 2 taken directly from the King James Version bible in 1249 characters or less
```
# try using length of 295
```
Generate passionate, meaningful, heartfelt, and profound lyrics to a full song inspired by and devoted to preserving the message of 1 Thessalonians 2 taken directly from the King James Version bible with remnants of the Gospel of Jesus Christ using at least 1200 but no more than 1249 characters
```

# Custom Lyrics Max Length: 1250

```
zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz
```
# try using lyrics inspired by the message of Galatians 6 from the King James Version bible (length is 1225)
```
(Verse 1)
In the fields of grace, where the wild winds blow,
We sow our seeds of faith, and watch them grow.
Beneath the moon's soft glow, and the starry sky,
We lift our burdens high, to the One on high.

(Chorus)
For in due season, we'll reap if we faint not,
Let us not grow weary in the good we've sought.
Let us do good unto all, as opportunity we seize,
For the Spirit's fruit shall abound, in love and peace.

(Verse 2)
With hearts intertwined, in the bonds of love,
We carry one another, to the heavens above.
With hands that toil, and hearts that pray,
We journey together, on this narrow way.

(Bridge)
Though the road be long, and the night be dark,
We'll press on forward, with hope's bright spark.
For the Lord is our strength, and our guiding light,
He leads us onward, through the darkest night.

(Chorus)
For in due season, we'll reap if we faint not,
Let us not grow weary in the good we've sought.
Let us do good unto all, as opportunity we seize,
For the Spirit's fruit shall abound, in love and peace.

(Outro)
In the fields of grace, where the wild winds blow,
We sow our seeds of faith, and watch them grow.
Beneath the moon's soft glow, and the starry sky,
We lift our burdens high, to the One on high.
```
# OR try using length 870
```
In the garden of love, where the lilies bloom,
I found my beloved, amidst the sweet perfume.
His eyes like doves, filled with endless grace,
His arms around me, in an embrace.

Oh, the fragrance of love, fills the air,
As we dance together, without a care.
His voice, like music, soothes my soul,
In his presence, I am made whole.

Like the apple tree among the trees,
He is my refuge, my heart at ease.
His love, a banner over me,
In his embrace, I am free.

In the vineyards of love, we will roam,
Hand in hand, we'll journey home.
For his love is stronger than death,
With him, I'll take my final breath.

Oh, let me lean upon his breast,
And find in him my perfect rest.
For he is the Alpha and Omega,
My Savior, my Redeemer.

In the garden of love, we'll abide,
With him, forever by my side.
For his love endures forevermore,
In him, I've found what I'm living for.
```
# OR try using length 1175
```
In the bonds of brotherhood, we stand,
Guided by the Savior's loving hand.
With hearts ablaze and spirits bright,
We spread His gospel, shining light.

Through trials and tribulations, we press on,
For in His grace, we are made strong.
With love unfeigned, our message rings true,
Proclaiming His mercy, for me and you.

In Thessalonica's streets, we tread,
Sharing His word, our daily bread.
With fervent prayer and earnest plea,
We lead the lost to Calvary's tree.

Oh, the joy of seeing souls set free,
From sin's dark chains, they now break free.
In Christ alone, our hope secure,
For His salvation, we endure.

With gentle care and tender heart,
We nurture faith, we play our part.
For in the Gospel, power untold,
His love and mercy, ever bold.

So let us labor, night and day,
To spread His truth, come what may.
For in His vineyard, we are blessed,
To be His hands, His love expressed.

In 1 Thessalonians, our guide we find,
To love and serve, with heart and mind.
For in His word, our path is clear,
To share His love, without fear.

So let us walk, in faith and love,
Pointing others to heaven above.
For in His grace, we are set free,
To live and love, eternally.
```
# OR try using length 466
```
[Verse]
We walk in love
Spreading His grace
Guided by faith
In this holy place
Our hearts ablaze
With fervent fire
Spreading the word
Our one desire

We speak His truth
With gentle embrace
Challenging hearts
To seek His face
His love unending
His mercy profound
In Him alone
Our hope is found

[Verse 2]
Through trials and pain
We proclaim His name
His love abounds
There's no greater fame
United we stand
In joyful refrain
Proclaiming His truth
We break every chain
```

# Custom Style of Music Max Length: 120
```
zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz
```
# try using length of 94
```
mongolian folk, D# Phrygian (Minor), male  Borbangnadyr singer, bass guitar
```
# OR using length of 111
```
progressive metal djent, Bb Mixolydian (Minor), male Khoomei Kharkhiraa Khoomei singer, guttural throat singing
```
# OR using length of 104
```
progressive metal djent, Db Mixolydian (Major), male Basso Profondo Bass singer, guttural throat singing
```
# OR using length of 113
```
mongolian folk metal, Bb Phrygian (Minor), lead female Coloratura Mezzo-Soprano singer, french horn accompaniment
```

# Simple Song Description Max Length: 200
```
zzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzzz
```
# try using length of 174
```
bluegrass gospel, D# Lydian (Major), lead male Countertenor Countertenor singer, accordion, lyrics inspired by the message of Revelation 20 from the King James Version bible
```
# OR length of 168
```
classical celtic guitar, Bb Aeolian (Minor), male Lyric Baritone singer, castanets, lyrics inspired by the message of Galatians 6 from the King James Version bible
```
# OR length of 198
```
classical celtic guitar, Bb Mixolydian (Minor), male Khoomei Kharkhiraa Khoomei singer, guttural throat singing, lyrics inspired by the message of Song of Solomon 6 from the King James Version bible
```
# OR length of 198
```
progressive metal djent, Db Mixolydian (Major), male Basso Profondo Bass singer, guttural throat singing, lyrics inspired by the message of 1 Thessalonians 5 from the King James Version bible
```
# OR length of 97
```
smooth vaporwave jazz lo-fi hip-hop, guttural throat singing, in the key of F# Mixolydian (Major)
```

# The King James Version (KJV) of the Bible is Public Domain and contains 66 books, divided into two main sections: the Old Testament and the New Testament. Here's a list of each book along with a brief description and the number of chapters in each:

```
    # List of tuples to store every Bible Book and total number of Chapters
    bible_chapters = [
        ("Genesis", 50),
        ("Exodus", 40),
        ("Leviticus", 27),
        ("Numbers", 36),
        ("Deuteronomy", 34),
        ("Joshua", 24),
        ("Judges", 21),
        ("Ruth", 4),
        ("1 Samuel", 31),
        ("2 Samuel", 24),
        ("1 Kings", 22),
        ("2 Kings", 25),
        ("1 Chronicles", 29),
        ("2 Chronicles", 36),
        ("Ezra", 10),
        ("Nehemiah", 13),
        ("Esther", 10),
        ("Job", 42),
        ("Psalms", 150),
        ("Proverbs", 31),
        ("Ecclesiastes", 12),
        ("Song of Solomon", 8),
        ("Isaiah", 66),
        ("Jeremiah", 52),
        ("Lamentations", 5),
        ("Ezekiel", 48),
        ("Daniel", 12),
        ("Hosea", 14),
        ("Joel", 3),
        ("Amos", 9),
        ("Obadiah", 1),
        ("Jonah", 4),
        ("Micah", 7),
        ("Nahum", 3),
        ("Habakkuk", 3),
        ("Zephaniah", 3),
        ("Haggai", 2),
        ("Zechariah", 14),
        ("Malachi", 4),
        ("Matthew", 28),
        ("Mark", 16),
        ("Luke", 24),
        ("John", 21),
        ("Acts", 28),
        ("Romans", 16),
        ("1 Corinthians", 16),
        ("2 Corinthians", 13),
        ("Galatians", 6),
        ("Ephesians", 6),
        ("Philippians", 4),
        ("Colossians", 4),
        ("1 Thessalonians", 5),
        ("2 Thessalonians", 3),
        ("1 Timothy", 6),
        ("2 Timothy", 4),
        ("Titus", 3),
        ("Philemon", 1),
        ("Hebrews", 13),
        ("James", 5),
        ("1 Peter", 5),
        ("2 Peter", 3),
        ("1 John", 5),
        ("2 John", 1),
        ("3 John", 1),
        ("Jude", 1),
        ("Revelation", 22)
    ]
```

# Old Testament:

# Genesis (50 chapters)
# This book begins with the creation story and covers the early history of mankind, including the patriarchs Abraham, Isaac, and Jacob.

# Exodus (40 chapters)
# Exodus narrates the liberation of the Israelites from slavery in Egypt, the receiving of the Ten Commandments, and the establishment of the covenant between God and Israel.

# Leviticus (27 chapters)
# Leviticus focuses on laws related to worship, purity, and morality, including regulations for sacrifices, offerings, and priestly conduct.

# Numbers (36 chapters)
# Numbers recounts the journey of the Israelites from Mount Sinai to the borders of the Promised Land, including the census of the Israelites and various laws.

# Deuteronomy (34 chapters)
# Deuteronomy consists largely of speeches by Moses, reviewing the laws and events of the Israelites' journey and preparing them for their entrance into the Promised Land.

# Joshua (24 chapters)
# Joshua details the conquest of Canaan under the leadership of Joshua, successor to Moses, and the division of the land among the tribes of Israel.

# Judges (21 chapters)
# Judges tells the stories of various leaders called judges who guided Israel before the time of the kings, often highlighting cycles of sin, oppression, repentance, and deliverance.

# Ruth (4 chapters)
# Ruth is a narrative of loyalty and faithfulness, centered on Ruth, a Moabite woman, who becomes the great-grandmother of King David.

# 1 Samuel (31 chapters)
# 1 Samuel describes the transition from the period of the judges to the monarchy in Israel, focusing on the lives of Samuel, Saul, and David.

# 2 Samuel (24 chapters)
# 2 Samuel continues the story of David's reign as king, including his victories, failures, and the establishment of the Davidic covenant.

# 1 Kings (22 chapters)
# 1 Kings covers the reigns of Solomon, the division of the kingdom after his death, and the history of the kings of Israel and Judah.

# 2 Kings (25 chapters)
# 2 Kings provides a continuation of the history of the divided kingdoms of Israel and Judah, including the fall of both kingdoms and the exile of the Israelites.

# 1 Chronicles (29 chapters)
# 1 Chronicles traces the genealogies of Israel and provides a selective history from Adam to King David, emphasizing David's reign.

# 2 Chronicles (36 chapters)
# 2 Chronicles focuses primarily on the reign of Solomon and the history of the kingdom of Judah, highlighting the importance of the temple and proper worship.

# Ezra (10 chapters)
# Ezra recounts the return of the exiled Israelites from Babylon to Jerusalem and the efforts to rebuild the temple.

# Nehemiah (13 chapters)
# Nehemiah continues the story of the restoration of Jerusalem, focusing on the efforts of Nehemiah to rebuild the city walls and restore the people's faithfulness to God's law.

# Esther (10 chapters)
# Esther tells the story of a Jewish girl who becomes queen of Persia and, with the help of her cousin Mordecai, saves her people from destruction.

# Job (42 chapters)
# Job explores the question of why the righteous suffer, focusing on the experiences of a man named Job who faces severe trials but maintains his faith in God.

# Psalms (150 chapters)
# Psalms is a collection of 150 poetic songs and prayers, expressing a wide range of human emotions and experiences, including praise, lament, thanksgiving, and trust in God.

# Proverbs (31 chapters)
# Proverbs contains wise sayings and instructions for living a godly and prudent life, often attributed to King Solomon.

# Ecclesiastes (12 chapters)
# Ecclesiastes reflects on the meaninglessness of life apart from God and emphasizes the importance of fearing God and obeying His commandments.

# Song of Solomon (8 chapters)
# Song of Solomon, also known as Song of Songs, is a collection of love poems celebrating the beauty of romantic love within marriage.

# Isaiah (66 chapters)
# Isaiah contains prophecies concerning the coming judgment on Israel and the nations, as well as promises of restoration and the coming Messiah.

# Jeremiah (52 chapters)
# Jeremiah prophesies the impending judgment on Judah for its disobedience to God, as well as the promise of restoration and the new covenant.

# Lamentations (5 chapters)
# Lamentations mourns the destruction of Jerusalem and the suffering of the people, yet it also expresses hope in God's faithfulness and mercy.

# Ezekiel (48 chapters)
# Ezekiel contains visions and prophecies concerning the judgment on Israel, the future restoration, and the coming of the kingdom of God.

# Daniel (12 chapters)
# Daniel features stories of faithfulness in the face of persecution, as well as apocalyptic visions concerning the future kingdoms and the ultimate victory of God.

# Hosea (14 chapters)
# Hosea prophesies against the idolatry and unfaithfulness of Israel, using his own troubled marriage as a metaphor for God's relationship with His people.

# Joel (3 chapters)
# Joel calls for repentance in the face of an impending locust plague, while also prophesying future judgment and restoration.

# Amos (9 chapters)
# Amos denounces the social injustices and religious hypocrisy of Israel, warning of the coming judgment and calling for repentance.

# Obadiah (1 chapter)
# Obadiah pronounces judgment against the nation of Edom for its violence against Israel and predicts its eventual downfall.

# Jonah (4 chapters)
# Jonah tells the story of a reluctant prophet sent to preach to the city of Nineveh, highlighting God's mercy and concern for all peoples.

# Micah (7 chapters)
# Micah condemns the corruption and injustice in Israel and Judah, while also offering hope for a future restoration under a righteous ruler.

# Nahum (3 chapters)
# Nahum prophesies the destruction of Nineveh, the capital of Assyria, as a judgment for its violence and oppression.

# Habakkuk (3 chapters)
# Habakkuk questions God's justice in the face of evil and violence but ultimately expresses trust and confidence in God's sovereignty.

# Zephaniah (3 chapters)
# Zephaniah warns of the coming judgment on Judah and the nations, yet also offers hope of restoration for a remnant of God's people.

# New Testament:

# Matthew (28 chapters)
# Matthew presents Jesus as the fulfillment of Old Testament prophecies, focusing on His teachings, miracles, and the establishment of the kingdom of God.

# Mark (16 chapters)
# Mark emphasizes Jesus' actions and His role as the suffering servant, highlighting His miracles and the significance of His death and resurrection.

# Luke (24 chapters)
# Luke provides a detailed account of Jesus' life, ministry, death, and resurrection, with an emphasis on His compassion for the marginalized and His universal message of salvation.

# John (21 chapters)
# John focuses on the divinity of Jesus, presenting Him as the eternal Word made flesh and emphasizing the importance of faith in Him for eternal life.

# Acts (28 chapters)
# Acts narrates the growth of the early Christian church, from the Day of Pentecost to Paul's missionary journeys and eventual imprisonment in Rome.

# Romans (16 chapters)
# Romans explains the gospel message of salvation by grace through faith in Jesus Christ, emphasizing the righteousness of God and the universal need for redemption.

# 1 Corinthians (16 chapters)
# 1 Corinthians addresses various issues within the Corinthian church, including divisions, immorality, lawsuits, and proper conduct in worship.

# 2 Corinthians (13 chapters)
# 2 Corinthians is Paul's follow-up letter to the Corinthians, defending his apostolic authority and addressing challenges and criticisms he faced.

# Galatians (6 chapters)
# Galatians argues against the necessity of circumcision and observance of the Mosaic law for salvation, emphasizing justification by faith alone.

# Ephesians (6 chapters)
# Ephesians highlights the unity of believers in Christ and describes the spiritual blessings and responsibilities of being part of God's family.

# Philippians (4 chapters)
# Philippians expresses joy and gratitude amidst suffering and encourages believers to have the mindset of Christ, focusing on humility, unity, and perseverance.

# Colossians (4 chapters)
# Colossians warns against false teachings and emphasizes the supremacy of Christ, urging believers to live in accordance with their identity in Him.

# 1 Thessalonians (5 chapters)
# 1 Thessalonians encourages believers in their faithfulness amidst persecution and addresses questions about Christ's return.

# 2 Thessalonians (3 chapters)
# 2 Thessalonians addresses misunderstandings about Christ's return and encourages believers to stand firm in their faith.

# 1 Timothy (6 chapters)
# 1 Timothy provides instructions for church leadership and conduct, addressing issues such as false teaching, prayer, and the role of women.

# 2 Timothy (4 chapters)
# 2 Timothy is Paul's final letter, written to encourage and instruct Timothy in his ministry and to urge him to remain faithful in the face of challenges.

# Titus (3 chapters)
# Titus contains instructions for appointing elders, maintaining sound doctrine, and living in a manner consistent with the gospel.

# Philemon (1 chapter)
# Philemon is a personal letter from Paul to Philemon, urging him to forgive his runaway slave Onesimus and to receive him back as a brother in Christ.

# Hebrews (13 chapters)
# Hebrews presents Jesus as the ultimate High Priest and mediator of a better covenant, encouraging believers to persevere in faith and not to return to Judaism.

# James (5 chapters)
# James emphasizes the importance of genuine faith, expressed through good works and practical wisdom in daily life.

# 1 Peter (5 chapters)
# 1 Peter encourages believers to endure suffering with hope and to live as holy witnesses in a hostile world, focusing on the future inheritance awaiting them.

# 2 Peter (3 chapters)
# 2 Peter warns against false teachers and encourages believers to grow in knowledge and to remain steadfast in their faith.

# 1 John (5 chapters)
# 1 John emphasizes the importance of love, obedience, and fellowship with God, with a focus on the assurance of salvation and the reality of Christ's incarnation.

# 2 John (1 chapter)
# 2 John warns against false teachers and emphasizes the importance of truth and love in the Christian life.

# 3 John (1 chapter)
# 3 John commends hospitality and support for faithful ministers while warning against the arrogance and hostility of Diotrephes.

# Jude (1 chapter)
# Jude warns against false teachers and encourages believers to contend earnestly for the faith once for all delivered to the saints.

# Revelation (22 chapters)
# Revelation contains apocalyptic visions of the future, including the return of Christ, the final judgment, and the establishment of God's eternal kingdom.


# In Western music, a musical key refers to a set of notes and chords that revolve around a central note, called the tonic. Each key can be associated with one of the seven diatonic modes, which are scales that are derived from the major scale. The seven diatonic modes are:

# Ionian mode: This is equivalent to the major scale.
# Dorian mode: It is similar to the natural minor scale but with a raised sixth degree.
# Phrygian mode: It is similar to the natural minor scale but with a lowered second degree.
# Lydian mode: It is similar to the major scale but with a raised fourth degree.
# Mixolydian mode: It is similar to the major scale but with a lowered seventh degree.
# Aeolian mode: This is equivalent to the natural minor scale.
# Locrian mode: It is similar to the natural minor scale but with a lowered second and fifth degree.

# Here's a list of all the musical keys along with their associated modes:

```
keys = [
    ("C Ionian", "C", "Major", "Ionian"),
    ("C# Ionian", "C#", "Major", "Ionian"),
    ("Db Ionian", "Db", "Major", "Ionian"),
    ("D Ionian", "D", "Major", "Ionian"),
    ("D# Ionian", "D#", "Major", "Ionian"),
    ("Eb Ionian", "Eb", "Major", "Ionian"),
    ("E Ionian", "E", "Major", "Ionian"),
    ("F Ionian", "F", "Major", "Ionian"),
    ("F# Ionian", "F#", "Major", "Ionian"),
    ("Gb Ionian", "Gb", "Major", "Ionian"),
    ("G Ionian", "G", "Major", "Ionian"),
    ("G# Ionian", "G#", "Major", "Ionian"),
    ("Ab Ionian", "Ab", "Major", "Ionian"),
    ("A Ionian", "A", "Major", "Ionian"),
    ("A# Ionian", "A#", "Major", "Ionian"),
    ("Bb Ionian", "Bb", "Major", "Ionian"),
    ("B Ionian", "B", "Major", "Ionian"),
    ("C Dorian", "C", "Minor", "Dorian"),
    ("C# Dorian", "C#", "Minor", "Dorian"),
    ("Db Dorian", "Db", "Minor", "Dorian"),
    ("D Dorian", "D", "Minor", "Dorian"),
    ("D# Dorian", "D#", "Minor", "Dorian"),
    ("Eb Dorian", "Eb", "Minor", "Dorian"),
    ("E Dorian", "E", "Minor", "Dorian"),
    ("F Dorian", "F", "Minor", "Dorian"),
    ("F# Dorian", "F#", "Minor", "Dorian"),
    ("Gb Dorian", "Gb", "Minor", "Dorian"),
    ("G Dorian", "G", "Minor", "Dorian"),
    ("G# Dorian", "G#", "Minor", "Dorian"),
    ("Ab Dorian", "Ab", "Minor", "Dorian"),
    ("A Dorian", "A", "Minor", "Dorian"),
    ("A# Dorian", "A#", "Minor", "Dorian"),
    ("Bb Dorian", "Bb", "Minor", "Dorian"),
    ("B Dorian", "B", "Minor", "Dorian"),
    ("C Phrygian", "C", "Minor", "Phrygian"),
    ("C# Phrygian", "C#", "Minor", "Phrygian"),
    ("Db Phrygian", "Db", "Minor", "Phrygian"),
    ("D Phrygian", "D", "Minor", "Phrygian"),
    ("D# Phrygian", "D#", "Minor", "Phrygian"),
    ("Eb Phrygian", "Eb", "Minor", "Phrygian"),
    ("E Phrygian", "E", "Minor", "Phrygian"),
    ("F Phrygian", "F", "Minor", "Phrygian"),
    ("F# Phrygian", "F#", "Minor", "Phrygian"),
    ("Gb Phrygian", "Gb", "Minor", "Phrygian"),
    ("G Phrygian", "G", "Minor", "Phrygian"),
    ("G# Phrygian", "G#", "Minor", "Phrygian"),
    ("Ab Phrygian", "Ab", "Minor", "Phrygian"),
    ("A Phrygian", "A", "Minor", "Phrygian"),
    ("A# Phrygian", "A#", "Minor", "Phrygian"),
    ("Bb Phrygian", "Bb", "Minor", "Phrygian"),
    ("B Phrygian", "B", "Minor", "Phrygian"),
    ("C Lydian", "C", "Major", "Lydian"),
    ("C# Lydian", "C#", "Major", "Lydian"),
    ("Db Lydian", "Db", "Major", "Lydian"),
    ("D Lydian", "D", "Major", "Lydian"),
    ("D# Lydian", "D#", "Major", "Lydian"),
    ("Eb Lydian", "Eb", "Major", "Lydian"),
    ("E Lydian", "E", "Major", "Lydian"),
    ("F Lydian", "F", "Major", "Lydian"),
    ("F# Lydian", "F#", "Major", "Lydian"),
    ("Gb Lydian", "Gb", "Major", "Lydian"),
    ("G Lydian", "G", "Major", "Lydian"),
    ("G# Lydian", "G#", "Major", "Lydian"),
    ("Ab Lydian", "Ab", "Major", "Lydian"),
    ("A Lydian", "A", "Major", "Lydian"),
    ("A# Lydian", "A#", "Major", "Lydian"),
    ("Bb Lydian", "Bb", "Major", "Lydian"),
    ("B Lydian", "B", "Major", "Lydian"),
    ("C Mixolydian", "C", "Major", "Mixolydian"),
    ("C# Mixolydian", "C#", "Major", "Mixolydian"),
    ("Db Mixolydian", "Db", "Major", "Mixolydian"),
    ("D Mixolydian", "D", "Major", "Mixolydian"),
    ("D# Mixolydian", "D#", "Major", "Mixolydian"),
    ("Eb Mixolydian", "Eb", "Major", "Mixolydian"),
    ("E Mixolydian", "E", "Major", "Mixolydian"),
    ("F Mixolydian", "F", "Major", "Mixolydian"),
    ("F# Mixolydian", "F#", "Major", "Mixolydian"),
    ("Gb Mixolydian", "Gb", "Major", "Mixolydian"),
    ("G Mixolydian", "G", "Major", "Mixolydian"),
    ("G# Mixolydian", "G#", "Major", "Mixolydian"),
    ("Ab Mixolydian", "Ab", "Major", "Mixolydian"),
    ("A Mixolydian", "A", "Major", "Mixolydian"),
    ("A# Mixolydian", "A#", "Major", "Mixolydian"),
    ("Bb Mixolydian", "Bb", "Major", "Mixolydian"),
    ("B Mixolydian", "B", "Major", "Mixolydian"),
    ("C Aeolian", "C", "Minor", "Aeolian"),
    ("C# Aeolian", "C#", "Minor", "Aeolian"),
    ("Db Aeolian", "Db", "Minor", "Aeolian"),
    ("D Aeolian", "D", "Minor", "Aeolian"),
    ("D# Aeolian", "D#", "Minor", "Aeolian"),
    ("Eb Aeolian", "Eb", "Minor", "Aeolian"),
    ("E Aeolian", "E", "Minor", "Aeolian"),
    ("F Aeolian", "F", "Minor", "Aeolian"),
    ("F# Aeolian", "F#", "Minor", "Aeolian"),
    ("Gb Aeolian", "Gb", "Minor", "Aeolian"),
    ("G Aeolian", "G", "Minor", "Aeolian"),
    ("G# Aeolian", "G#", "Minor", "Aeolian"),
    ("Ab Aeolian", "Ab", "Minor", "Aeolian"),
    ("A Aeolian", "A", "Minor", "Aeolian"),
    ("A# Aeolian", "A#", "Minor", "Aeolian"),
    ("Bb Aeolian", "Bb", "Minor", "Aeolian"),
    ("B Aeolian", "B", "Minor", "Aeolian"),
    ("C Locrian", "C", "Minor", "Locrian"),
    ("C# Locrian", "C#", "Minor", "Locrian"),
    ("Db Locrian", "Db", "Minor", "Locrian"),
    ("D Locrian", "D", "Minor", "Locrian"),
    ("D# Locrian", "D#", "Minor", "Locrian"),
    ("Eb Locrian", "Eb", "Minor", "Locrian"),
    ("E Locrian", "E", "Minor", "Locrian"),
    ("F Locrian", "F", "Minor", "Locrian"),
    ("F# Locrian", "F#", "Minor", "Locrian"),
    ("Gb Locrian", "Gb", "Minor", "Locrian"),
    ("G Locrian", "G", "Minor", "Locrian"),
    ("G# Locrian", "G#", "Minor", "Locrian"),
    ("Ab Locrian", "Ab", "Minor", "Locrian"),
    ("A Locrian", "A", "Minor", "Locrian"),
    ("A# Locrian", "A#", "Minor", "Locrian"),
    ("Bb Locrian", "Bb", "Minor", "Locrian"),
    ("B Locrian", "B", "Minor", "Locrian")
]
```

# Each key can be played using any of the seven diatonic modes, but traditionally, each mode is associated with a particular starting note (or tonic), as listed above.

# list of different types of vocalists, categorized by vocal range and voice type:
```
vocal_types = [
    # Female Vocal Types
    ("Soprano", "Coloratura", "female"),
    ("Soprano", "Lyric", "female"),
    ("Soprano", "Dramatic", "female"),
    ("Mezzo-Soprano", "Coloratura", "female"),
    ("Mezzo-Soprano", "Lyric", "female"),
    ("Mezzo-Soprano", "Dramatic", "female"),
    ("Contralto", "Alto", "female"),
    
    # Male Vocal Types
    ("Countertenor", "Countertenor", "male"), # (male alto, often associated with falsetto)
    ("Tenor", "Leggero", "male"),
    ("Tenor", "Lyric", "male"),
    ("Tenor", "Spinto", "male"),
    ("Tenor", "Dramatic", "male"),
    ("Baritone", "Lyric", "male"),
    ("Baritone", "Dramatic", "male"),
    ("Bass", "Bass-Baritone", "male"),
    ("Bass", "Basso Profondo", "male"),
    ("Bass", "Lyric", "male"),
    ("Bass", "Dramatic", "male")
]
```

# Each of these categories can further be broken down into more specific subtypes based on vocal agility, timbre, and other characteristics.

# Mongolian throat singing, also known as Khöömei or Overtone singing, encompasses various styles and techniques. Here are some types of Mongolian throat singing:

# Khoomei (Khöömei): The most well-known style of Mongolian throat singing, characterized by producing multiple pitches simultaneously. It includes subtypes such as:
# Kharkhiraa Khoomei: Known for its high-pitched and piercing sounds.
# Khoomei (Tuvan Style): Originating from the Tuva region of Russia, this style involves producing deep, resonant tones.
# Sygyt: A style of overtone singing where the singer produces a clear, flute-like sound with harmonics.
# Kargyraa: Involves producing a deep, growling sound with overtone resonance.
# Borbangnadyr: Combines elements of Khoomei and Kargyraa, resulting in a pulsating rhythm with harmonic overtones.
# Ezengileer: A style that emphasizes nasal resonance, creating a unique timbre.
# Chylandyk: Originating from the Altai region, this style involves producing high-pitched, bird-like sounds.
```
mongolian_throat_singing_styles = [
    ("Khoomei (Khöömei)", "Kharkhiraa Khoomei"),
    ("Khoomei (Khöömei)", "Tuvan Style"),
    ("Sygyt", None),
    ("Kargyraa", None),
    ("Borbangnadyr", None),
    ("Ezengileer", None),
    ("Chylandyk", None)
]
```

# List of instruments
```
    # This tuple contains the names of various musical instruments.
    instruments = [
        ("piano"),
        ("guitar"),
        ("violin"),
        ("flute"),
        ("trumpet"),
        ("drums"),
        ("saxophone"),
        ("cello"),
        ("clarinet"),
        ("bass guitar"),
        ("accordion"),
        ("harp"),
        ("trombone"),
        ("ukulele"),
        ("banjo"),
        ("double bass"),
        ("harmonica"),
        ("mandolin"),
        ("xylophone"),
        ("oboe"),
        ("electric guitar"),
        ("bassoon"),
        ("french horn"),
        ("synthesizer"),
        ("accordion"),
        ("bagpipes"),
        ("conga"),
        ("djembe"),
        ("marimba"),
        ("organ"),
        ("steel drum"),
        ("tabla"),
        ("tambourine"),
        ("triangle"),
        ("vibraphone"),
        ("zither"),
        ("cello"),
        ("bongo"),
        ("castanets"),
        ("cowbell"),
        ("didgeridoo"),
        ("kazoo"),
        ("tuba"),
        ("fiddle"),
        ("harp"),
        ("drums"),
        ("guttural throat singing"),
        ("mongolian guitar"),
        ("horsehead fiddle")
    ]
```

# List of musical genres where True is for instrumental generation
```
    # A list of tuples representing song genre
    song_genre = [
        ("classical acoustic guitar", True),
        ("progressive metal djent", True),
        ("classical acoustic guitar melody", True),
        ("classical celtic guitar melody", True),
        ("fast aggressive phonk", True),
        ("slow ambient drone", True),
        ("heavy metal", True),
        ("fast jazz fusion", True),
        ("heavy electronic dance music", True),
        ("slow reggae", True),
        ("heavy ambient drone", True),
        ("slow country folk", True),
        ("fast hip-hop", True),
        ("fast salsa", True),
        ("fast bluegrass", True),
        ("fast screamo", True),
        ("slow indie rock", True),
        ("fast reggaeton", True),
        ("fast progressive house", True),
        ("fast trap", True),
        ("slow psychedelic rock", True),
        ("fast techno", True),
        ("slow blues", True),
        ("slow R&B", True),
        ("fast punk rock", True),
        ("heavy dubstep", True),
        ("fast thrash metal", True),
        ("slow bossa nova", True),
        ("fast disco", True),
        ("heavy industrial", True),
        ("fast garage rock", True),
        ("slow folk ballad", True),
        ("fast drum and bass", True),
        ("heavy doom metal", True),
        ("fast grindcore", True),
        ("slow tango", True),
        ("fast flamenco", True),
        ("heavy death metal", True),
        ("fast breakbeat", True),
        ("slow waltz", True),
        ("fast hardcore punk", True),
        ("heavy sludge metal", True),
        ("slow soul", True),
        ("fast electroswing", True),
        ("heavy thrash metal", True),
        ("fast ska", True),
        ("slow chamber music", True),
        ("fast house", True),
        ("fast hardstyle", True),
        ("kpop", True),
        ("minimalist techno", True),
        ("darkwave", True),
        ("acid jazz", True),
        ("neofolk", True),
        ("chiptune", True),
        ("witch house", True),
        ("noise rock", True),
        ("IDM (Intelligent Dance Music)", True),
        ("shoegaze", True),
        ("vaporwave", True),
        ("zydeco", True),
        ("krautrock", True),
        ("powernoise", True),
        ("glitch", True),
        ("wonky", True),
        ("chillwave", True),
        ("future garage", True),
        ("post-rock", True),
        ("math rock", True),
        ("jungle", True),
        ("breakcore", True),
        ("lo-fi hip hop", True),
        ("lo-fi indie", True),
        ("lo-fi house", True),
        ("haunting atmospheric witch house", True),
        ("fast aggressive witch house", True),
        ("lo-fi hip-hop", True),
        ("smooth vaporwave jazz", True),
        ("smooth fusion jazz", True),
        ("smooth vaporwave jazz lo-fi hip-hop", True),
        ("mongolian folk", True),
        ("mongolian folk metal", True),
        ("Chinese Classical folk", True),
        ("classical celtic guitar", True),
        ("symphonic metal", True),
        ("western", True),
        ("american folk", True)
    ]
```