# StudentWellbeing
Repository Created for Arefacts from the Student Wellbeing Specification Development Workshop 20th October, 2016.


## Aim:
To achieve a shared understanding of Student wellbeing information and an idea of
use cases for transmission of this information.

 

Note: SIF Objects
are primarily for the transmission of information between systems and not to
define the backend systems or entities.

From discussions entities involved could be:

##Students
– currently represented in SIF by
StudentPersonal.  The student is centric
for this area of information.  What
information needs to be carried with the student to meet a school’s ‘Duty of
Care’?  What information impacts on a
Student’s ability to succeed?  What
information is needed for mandatory reporting requirements to jurisdictions and
other agencies?

##Parents/Contacts
– currently represented in SIF by
StudentContact and StudentContactRelationship

##Teachers
– currently represented in SIF by StaffPersonal.

##Core Wellbeing Characteristic
that is integral to the
Student.  Be that a Medical condition or
a characteristic such as a known disability or any other characteristic or
condition that is student specific and impacts their learning.  

##Legal Order
– circumstance that effects the student but from an
outside influence  e.g. Custody or
Intervention Orders etc.  The impact on
the student is through the entity that is intrinsic to this 

##Pastoral Care Record
– Information relating to a
student that can impact on a student’s duty of care, special needs, includes
demographics and student background information.  Information of this nature can and will be
contained more broadly in Student Demographic and PersonalInfo containers
already in the SIF Specification, however, this entity is for recording extra
information outside of that which is currently collected.  E.g. Special Needs, details of any
integration aides required or other information or support that impacts on a
student’s ability to succeed in school or impacts their learning and needs to
be transferred to other systems.  A lot
of this information may remain in the 3rd party innovation system.

##Student Behaviour Event (Wellbeing
Incident)
- Student Behaviour – Event that impacts on a student’s duty of
care.  This has been modelled by Sentral
as an Incident, by CEOM as a behaviour support incident and by WA previously an
"Incident Report" but looking to move to terminology such as a “behaviour
record”.  In the room, there was an
emphasis that this ‘event’ was needed to track both ‘positive’ and ‘negative’
behaviours and it not just the recording of a discipline incident or an accident.

##Consequences
–  Actions -
 a Student Behavioural Event – or more
often referred to in discussions as an ‘Incident’ usually will have a
consequence, action or an outcome.  Many
may have consequences that need to be reported to other systems or
agencies.  This may be a Suspension, an
Expulsion or an experience which requires reward or recognition.

##Individualised Student Plans
– result of a Core Characteristic,
Legal order, Pastoral Care info, ability or Student Behaviour.  Extensive area and need to note in SIF only
that information that needs to be transferred between systems or agencies.  Two main broad categories of Learning Plans
have been identified as a Medical Plan and a Student Learning Plan.

##Alerts
–both– Medical – legal – requiring intervention or
knowledge.  The need for something that
can be sent, associated with the student to transfer information that carries
basic, important information. 
Lightweight, it needs to alert teachers and systems that this student
has a ‘concern’ that needs to be known for ‘duty of care’.  Currently in the SIF Model there exists the
concept of ‘medical alerts’ and ‘alerts’ but these are lists of events that are
carried with StudentPersonal and if anything is changed then for it to be
recognised by consuming systems, they would need to re-consume StudentPersonal
and ALL of the lists of alerts.  It was
noted that this information needs to travel as the result of an event not
necessarily as a by-product of a change in StudentPersonal.

##Diagram

![Wellbeingentity](https://github.com/nsip/StudentWellBeing/blob/master/Wellbeingentity.png)



