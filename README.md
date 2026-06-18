# Final_exam_RalphTheophile
Final Exam Project.
# Final Exam Practical - ITDI204 Cloud Computing

## Student information

**Student name:** Ralph Theophile

**GitHub repository URL:** https://github.com/Ralph-678/Final_exam_RalphTheophile.git 

**Render application URL/production:** https://final-exam-ralphtheophile-production.onrender.com 
**Render application URL/staging:** https://final-exam-ralphtheophile-staging.onrender.com 

---

## Application information

**Application name:** Final Exam - Ralph Theophile

**Render project name:** Final Exam - Ralph Theophile

**Branch used for production deployment:** **main**

**Staging branch name:** **staging**

---

## Deployment configuration(Production)

**Build command:** **npm install**

**Start command:** **npm start**

**Environment variable MSG:** **Final Exam**

**Environment variable ENV:** **Production**
## Deployment configuration(Staging)

**Build command:** **npm install**

**Start command:** **npm start**

**Environment variable MSG:** **Final Exam**

**Environment variable ENV:** **Staging**

---

## API endpoints to test

### Presentation endpoint

**URL:** https://final-exam-ralphtheophile-production.onrender.com/presentation

**Expected result:** Final Exam - Production

### Correction endpoint

**URL:** https://final-exam-ralphtheophile-production.onrender.com/correction 

**Error after first call:** Internal Server Error

**Expected result after correction:** Correction endpoint is working

---

## Error detection

Briefly explain what you corrected and how you moved the correction from staging to production.

**Explanation:**  
it was a wrong typo that couses an Internal server Error. on the Api route in was written res.sen insted of res.send. after updating the typo i did a git add to add the current change and a git -m adding the message than git push the the staging branch test with the ci/cd pipline than test with the staging services on render by deploying the latest commit. after ensuring everithing works we mergi it into the main branch ready fo the deployment in production service.

What is the other way you could have detected there were an error in the code without testing the API enpoints?

**Explanation:** 
the other way to detected that there were an error, is the action bar in GiutHub the 
CI/CD pipeline. that action will detect automaticaly when there is an error.