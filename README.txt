Υλοποίηση Συστημάτων Βάσεων Δεδομένων 2019-20
Άσκηση 3

Όνομα                         Α.Μ.
-------------------------------------------
Κρυπωτός Χρήστος              1115201700063
Παπαδάκος Λεωνίδας-Παναγιώτης 1115201700117

================================================================================

Παραδοχές:

[*] Οι συναρτήσεις επιπέδου ΑΜ επιστρέφουν AME_ERROR σε περίπτωση σφάλματος και
    θέτουν κωδικό σφάλματος στο AM_errno. Η εκφώνηση ορίζει την AM_PrintError.
    (Παρόμοια λογική με errno)

[*] H AM_FindNextEntry επιστρέφει pointer σε σημείο ενός BF_Block κάπου στη
    μνήμη. Γι'αυτό κάνει unpin το μπλοκ μόνο όταν δεν το χρειάζεται πια, ώστε
    να παραμείνουν τα σωστά δεδομένα (το δεύτερο πεδίο ενός record) στη θέση
    μνήμης όπου δείχνει.

[*] Το split ανταπωκρίνεται στις υποθέσεις και τα test cases της εργασίας.
