# ΙΟΝΙΟ ΠΑΝΕΠΙΣΤΗΜΙΟ
# ΤΜΗΜΑΤΟΣ ΠΛΗΡΟΦΟΡΙΚΗΣ 
# ΜΑΘΗΜΑ: Επικοινωνία Ανθρώπου Υπολογιστή

Φοιτητής:

Γεωργίου Ορφέας - Π2015033 - p15geor1@ionio.gr

Κέρκυρα, 2016

##Σύνοψη

Η κρυπτογραφία είναι ο θεμέλιος λίθος της ασφάλειας των υπολογιστών και αποτελεί ιδιαίτερα ενδιαφέρον αντικείμενο για 
πειραματική ενασχόληση σε μεγάλο εύρος ηλικιών. Με το παρόν παιχνίδι δίνεται η δυνατότητα σε χρήστες μικρότερων ηλικιών
να έρθουν σε επαφή με την κρυπτογραφία και πιο συγκεκριμένα με τον απλό αλγόριθμο του Καίσαρα.

#Εισαγωγή 

#Περιγραφή gameplay του παιχνιδιού.
Το αεροπλάνο του χρήστη έχει ως βασική αποστολή να πυροβολήσει επανειλημμένα τις δυο ταμπέλες(θετική ή αρνητική) του γιγάντιου εχθρικού
αεροπλάνου και ως δευτερεύον να πυροβολήσει τα μικρότερα εχθρικά αεροπλάνα για να μπορέσει να επιβιώσει. Οσο συνεχίζει να πυροβολεί τις
ταμπέλες, το κρυπτομήνυμα κανει shift δεξιά ή αριστερά αντίστοιχα με την ταμπέλα που χτυπάει. Αν τα καταφέρει να κάνει αρκετές φορές shift
θα μπορέσει να εμφανίσει το μήνυμα του εχθρού και να νικήσει το παιχνίδι. Τα εχθρικά αεροπλάνα είναι ιδιαίτερα επικίνδυνα καθώς πυροβολούν
αλλά μπορούν και να συγκρουστούν με το αεροπλάνο του χρήστη για αυτό ο χρήστης έχει τη δυνατότητα να τα αποκρούσει κατεβαίνοντας με το 
αεροπλάνο σε πιο χαμηλό ύψος. Αν αυτό συμβεί τρείς φορές πριν ο χρήστης βρει το κατάλληλο μήνυμα τότε το αεροπλάνο καταστρέφεται και το 
παιχνίδι τερματίζει.

#Αφήγηση 
Η αφήγηση του παιχνιδιού έχει αλλάξει λίγο μόνο απο το κλασικό και πετυχημένο παιχνίδι στο οποίο βασίστηκε. Ωστόσο, τα στοιχεία που προστέθηκαν,
επιτρέπουν στο χρήστη να καταλάβει τον κόσμο στον οποίο βρίσκεται και την αποστολή που καλείται να αντιμετωπίσει. Βρισκόμαστε στην περίοδο του 
δευτέρου Παγκοσμίου Πολέμου και ο Alan Turing, ο οποίος βρίσκεται μέσα στο αεροπλάνο του χρήστη, προσπαθεί να βρεί τον κωδικό των εχθρών για να 
κερδιθεί ο πόλεμος. Το αεροπλάνο των εχθρών χλευάζει τον χρήστη και του δημιουργεί το κίνητρο να νικήσει το παιχνίδι. Ο χρήστης ταυτίζεται 
με τον Alan Turing και βάζει τα δυνατά του για να τον βοηθήσει. Τέλος, με χιουμουριστικό τρόπο μετα το λήξη του παιχνιδιού(αν κερδίσει ο παίκτης) 
εμφανίζεται ο Alan Turing να επαινεί τον χρήστη.

#Διαχείριση λάθους
Αρχικά, ο τρόπος με τον οποίο είχα αποφασίσει να κάνω τη διαχείριση λάθους ήταν η υπόδειξη του σωστού αριθμού των shift που χρειαζόταν για 
να κερδιθεί το παιχνίδι και επανέφερα το μήνυμα στην αρχική του μορφή παρά τις όποιες αλλαγές είχε καταφέρει ο χρήστης. Αργότερα 
συνειδητοποίησα ότι αυτό δεν δίνει τη δυνατότητα στο χρήστη να φτάσει πιο κοντά στη λύση. Η διαχείριση λάθους που επέλεξα αργότερα, είναι 
να μην εμφανίζεται ο απαιτούμενος αριθμός shift, αλλά να παραμένει το μήνυμα όπως ήταν πρωτού καταστραφεί το αεροπλάνο του χρήστη.
Με αυτόν τον τρόπο, μετα την καταστροφή του αεροπλάνου, ο χρήστης μπορεί να φτάνει πιο κοντά στην ήττα αλλά δεν χάνει καθόλου απο την πρόοδο
την οποία έχει κάνει.

#Προδιαγραφές Caesar 1942
* Ανθρωπος: Απευθύνεται κυρίως σε μαθήτες λυκείου και γυμνασίου(που θα έχουν αρκετά ανεπτυγμένη αντίληψη) για να κατανοήσουν τον τρόπο
  που λειτουργεί ο αλγόριθμος του Καίσαρα. Απαιτούνται βασικές γνώσεις υπολογιστή.
* Πλαίσιο χρήσης: Το παιχνίδι μπορεί να χρησιμοποιηθεί τόσο μέσα σε σχολική αίθουσα για την πιο ευχάριστη και ενδιαφέρουσα παρουσίαση του 
 αλγορίθμου, όσο και στο σπίτι, για καλύτερη κατανόηση.
* Σκοπός: Μια πρώτη επαφή με την κρυπτογραφία και κατανόηση του κρυπτογραφικού αλγορίθμου του Καίσαρα.
* Διεργασία χρήσης: Η διεργασία χρήσης είναι απλή και γίνεται με τα τέσσερα βελάκια για τις αντίστοιχες κινήσεις.
 Επίσης με τα πλήκτρα space πυροβολεί και με το s χαμηλώνει το ύψος του αεροπλάνου.
* Λόγοι επιτυχίας ή αποτυχίας: Βασίζεται σε ένα δοκιμασμένο κλασικό παιχνίδι το οποίο είχε επιτυχία. Υπάρχει δυνατότητα διαχείρισης του 
 σφάλματος, πράγμα που το κάνει φιλικό προς τον χρήστη.
 
#Σενάριο χρήσης
 Ένας μαθητής λυκείου έδειξε ιδιαίτερο ενδιαφέρον στις εφαρμογές της πληροφορικής και ιδιαίτερα στην ασφάλεια. Αυτό τον οδήγησε με την 
 βοήθεια του καθηγητή του στην κρυπτογραφία και τους απλούς αλγορίθμους κρυπτογράφησης. Μέσα από το παιχνίδι που του σύστησε ο καθηγητής του 
 μπόρεσε με ευχάριστο τρόπο να μάθει τον τρόπο που δουλεύει ο αλγόριθμος του Καίσαρα. Οι ολισθήσεις που συμβαίνουν στη διάρκεια του παιχνιδιού 
 εξυπηρετούν την κατανόηση του αλγορίθμου.
 
#Επιλογή εργαλείων
* Scratch: Tο Scratch είναι μια διερμηνευόμενη δυναμική οπτική γλώσσα προγραμματισμού.
* Ζωγραφική της Microsoft: Χρησιμοποιήθηκε για απλή επεξεργασία εικόνων.
 
#Διαδικασία Ανάπτυξης
  Η αρχική ιδέα του παιχνιδιού ήρθε μετά την υπόδειξη του καθηγητή του μαθήματος ότι το πρώτο παιχνίδι που δημιούργησα είχε αδυναμίες και 
 δεν περιείχε βασικά χαρακτηριστικά που απαιτούνται για τη δημιουργία ενός σωστού παιχνιδιού για το μάθημα της Επικοινωνίας Ανθρώπου-Υπολογιστή.
 Μετά απο αναζήτηση στα κλασικά παιχνίδια που είχαν υποδειχτεί αλλά και την πιο προσεκτική παρατήρηση του "πρότυπου" παιχνιδιού gem game μου
 ήρθε η ιδέα να τροποποιήσω το gem game με θέμα την κρυπτογραφία. Όταν το επιχείρησα, είδα ότι τα χαρακτηριστηκά του δεν ήταν κατάλληλα
 για να προσαρμοστούν στο θέμα της κρυπτογραφίας. Το 1942 ήταν το παιχνίδι που μου κέντρισε το ενδιαφέρον λόγω του ονόματος του, καθώς εκείνη
 τη χρονολογία το θέμα της αποκρυπτογράφησης ήταν ιδιαίτερα κρίσιμο για την έκβαση του πολέμου. Έτσι προσπάθησα να προσαρμόσω το θέμα της 
 κρυπτογραφίας και του πιο απλού και διαχειρίσιμου αλγορίθμου στο συγκεκριμένο παιχνίδι. Δυστυχώς, λόγω του αρχικού παιχνιδιού, δεν μπόρεσα
 να πάρω feed-back για αυτό το παιχνίδι και όποιες κριτικές και αξιολογήσεις έγιναν μέσω τρίτων. 
  Το 1942 ήταν λοιπόν το κλασικό παιχνίδι που βασίστηκα και παρουσιάζεται στις παρακάτω εικόνες:
  [![1942a.png](https://s18.postimg.org/6a2h4g7m1/1942a.png)](https://postimg.org/image/x7we66s91/)
  μέσα στο παιχνίδι:
  [![1942b.png](https://s12.postimg.org/zdxzze9z1/1942b.png)](https://postimg.org/image/l7i945z3t/)
  
  Ενδεικτικές Οθόνες απο το τροποποιημένο παιχνίδι και το link: https://scratch.mit.edu/projects/134375306/#player
  
  Η αρχική εικόνα:
  [![1942a.png](https://s18.postimg.org/9ftx9vda1/1942a.png)](https://postimg.org/image/hlbz811it/)
  Αφήγηση παιχνιδιού:
  [![1942b.png](https://s15.postimg.org/y1twge03v/1942b.png)](https://postimg.org/image/vx9jfayh3/)
  Προσπάθεια του χρήστη να κάνει shift το κρυπτογραφημένο μήνυμα:
  [![1943c.png](https://s11.postimg.org/fvyxy4qmb/1943c.png)](https://postimg.org/image/oqzs8nfen/)
  Η οθόνης που εμφανίζει σε περίπτωση που ο χρήστης χάσει όλες τις ζωές:
  [![1942d.png](https://s11.postimg.org/e7npeo3ir/1942d.png)](https://postimg.org/image/9yizci09b/)
  Η οθόνη που εμφανίζει σε περίπτωση που ο χρήστης κερδίσει:
  [![1942e.png](https://s17.postimg.org/je907vs5r/1942e.png)](https://postimg.org/image/946l8n2a3/)
  
##Συμπεράσματα και προτάσεις για μελλοντικές βελτιώσεις:

##Συμπεράσματα: 
To Ceacar 1942 είναι ένα παιχνίδι το οποίο δίνει τη δυνατότητα σε μαθητές να έρθουν σε επικοινωνία με τον αλγόριθμο του
 Καίσαρα. Έχει γίνει προσπάθεια να συμπεριλάβει όλα τα βασικά χαρακτηριστικά που πρέπει να έχει ένα εκπαιδευτικό παιχνίδι, ωστόσο αναμένω
 την αξιολόγηση απο τον διδάσκοντα για βελτιώσεις.
 
##Βελτιώσεις:
Πιθανόν να υπάρχει ανάγκη για περισσότερα επίπεδα και επιλογή δυσκολίας του παιχνιδιού.
 
##Βιβλιογραφικές Πηγές
* Ο Προγραμματισμός της Διάδρασης, Κωνσταντίνος Χωριανόπουλος
* https://github.com/courses-ionio/hci/tree/master/projects_2016/P2016000/Final_Report
 
