# StudentWellbeing

***DEPRECATED (RETIRED)***

*This repository is obsolete and retired (archived). This is an unmantained repository.*

Repository Created for Arefacts from the Student Wellbeing Specification Development Workshop 20th October, 2016.


## Aim
To achieve a shared understanding of Student wellbeing information and an idea of use cases for transmission of this information.

## Note
SIF Objects are primarily for the transmission of information between systems used by different parties, and not to define the backend systems or entities.

From discussions entities involved could be:

## Students
– currently represented in SIF by StudentPersonal.  The student is central for this area of information.  What information needs to be carried with the student to meet a school’s ‘Duty of Care’?  What information impacts on a Student’s ability to succeed?  What information specific to the student is needed for mandatory reporting requirements to jurisdictions and other agencies?
## Parents/Contacts
– currently represented in SIF by StudentContactPersonal and StudentContactRelationship
## Teachers
– currently represented in SIF by StaffPersonal.
Core Wellbeing Characteristic that is integral to the Student.  This may be a Medical condition, special needs or a characteristic such as a known disability or any other characteristic or condition that is student specific and impacts their learning. Some characteristics are already captured in the Demographics container of StudentPersonal however this object allows for more complex and targeted information. 
## Legal Order
– external circumstance that affects the student e.g. Custody or Intervention Orders etc.  The impact on the student is through the entity (parent/contact) that is intrinsic to this.
## Pastoral Care Record
– Information relating to a student that can impact on a student’s duty of care or particular needs, includes demographics and student background information. Likely to act as a summary of information represented elsewhere in the Wellbeing data model, that can be transferred with a student to another school. Information of this nature can and will be contained more broadly in Student Demographic and PersonalInfo containers already in the SIF Specification, however, this entity is for recording extra information outside of that which is currently represented in SIF.  E.g. Special Needs, details of any integration aides required or other information or support that impacts on a student’s ability to succeed in school or impacts their learning and needs to be transferred to other systems.  A lot of this information may remain in the 3rd party innovation system.
## Wellbeing Event (aka Wellbeing Incident - Student Behaviour)
– Event that impacts on a student’s duty of care.  This has been modelled by Sentral as an Incident, by CEOM as a behaviour support incident and by WA previously an "Incident Report" but looking to move to terminology such as a “behaviour support record”.  In the room, there was an emphasis that this ‘event’ was needed to track both ‘positive’ and ‘negative’ behaviours and it not just the recording of a discipline incident or an accident.  This event is specific to a student, and is not global (e.g. a pandemic): where an event involves more than one student, they can be listed in the person’s involved.  Where the event has an impact on a student’s wellbeing an individual record for each student should be generated.  E.g. where a student is reporting that another student fell off his bike, then the reporting student is listed as a person involved.
## Wellbeing Response
–  An outcome of a Student Wellbeing Event – or more often referred to in discussions as an ‘Incident’ usually will have a WellbeingResponse, action or an outcome.  Many events may have WellbeingResponses that need to be reported to other systems or agencies.  This may be a Suspension, an Expulsion/Exclusion, or an experience which requires reward or recognition. WA has specific language around categories of suspension—e.g. they are legally constrained not to refer to expulsion of students.
## Personalised Student Plans
– result of a Core Characteristic, Legal order, Pastoral Care info, ability or Student Behaviour. Will be a document, and the feeling in the room was that SIF would most usefully capture metadata around the document. Plans can be specific to a domain, but are still expected to aggregate information gathered about student in disparate locations. Extensive area and need to note in SIF only that information that needs to be transferred between systems or agencies.  Broad categories of Learning Plans that have been identified so far are Medical Plan, Learning Plan, Attendance Plan and Behavioural Plan.
## Alerts
– Alert indicating further intervention or knowledge required with regard to a student, which could be Medical, Legal or other. Can reflect both long-term attributes of a student (Characteristics) and short-term attributes (e.g. resulting from Events). They fulfil the need for something that can be sent, associated with the student to transfer information that carries basic, important information.  Lightweight, it needs to alert teachers and systems that this student has a ‘concern’ that needs to be known for ‘duty of care’.  Currently in the SIF Model there exists the concept of ‘medical alerts’ and ‘alerts’, but these are lists of events that are carried with StudentPersonal: if anything is changed then for it to be recognised by consuming systems, they would need to re-consume StudentPersonal and ALL of the lists of alerts.  It was noted that this information needs to travel as the result of an event or a concern, not necessarily as a by-product of a change in StudentPersonal.
## Appeal
– Appeal is information about an “appeal” or a “request” in regard to a (negative/punitive) WellbeingResponse to a student event.


![Wellbeingentity](https://github.com/nsip/StudentWellBeing/blob/master/Wellbeingentity.png)



