# Comentarea codului



// initializarea variabilei - zile pina la deadline 

int d; // days until deadline




// if the student is at least 18 years of age

if (student.Age> = 18)

{

    // send meeting invitation to the student
    
         // se apeleaza functia de transmiterea a mesajelor ce primeste ca parametru datele studentului si datele despre invitatie
         
    notificationService.SendMessageTo(student, meetingInvitation);
    
}

else // if the student is younger than 18 years 

{

    // sends a meeting invitation to the student's legal guardian
    
        // se apeleaza functia de transmiterea a mesajelor ce primeste ca parametru datele parintilor si datele despre invitatie
        
    notificationService.SendMessageTo(student.Parent, meetingInvitation);
    
}


// student is eligible for blood donation

// in cazul in care virsta e mai mare ca 17 ani, greutatea mai mare ca 58 kg, si inaltimea mai mare de 1.55 m

if (student.Age >= 17 && student.Weight >= 58.0 && student.Height >= 1.55)

{

    //Se apeleaza functia de alertare, ce primeste ca parametru datele studentului
    
    ScheduleBloodDonatingSessionWith(student);
    
}

