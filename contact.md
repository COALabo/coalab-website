---
layout: default
title: Contact & Join
permalink: /contact/
---

# Contact & Join COALAB

We welcome inquiries about our research, collaboration opportunities, and applications to join our lab.

## Contact Information

### Lab Location
**COALAB - Computational and Applied Linguistics Laboratory**  
Science Building, Room 301  
123 University Avenue  
Toronto, ON M5S 1A1  
Canada

### General Inquiries
- **Email:** [contact@coalab.org](mailto:contact@coalab.org)
- **Phone:** +1 (555) 123-4567
- **Fax:** +1 (555) 123-4568

### Lab Office Hours
- **Monday-Friday:** 9:00 AM - 5:00 PM
- **By appointment only**

### Individual Contacts
- **Dr. Peter Awe (PI):** [peter.awe@coalab.org](mailto:peter.awe@coalab.org)
- **Dr. Maria Chen (Postdoc):** [maria.chen@coalab.org](mailto:maria.chen@coalab.org)
- **Dr. James Wilson (Postdoc):** [james.wilson@coalab.org](mailto:james.wilson@coalab.org)
- **Dr. Sarah Johnson (Postdoc):** [sarah.johnson@coalab.org](mailto:sarah.johnson@coalab.org)

## Join Our Lab
<a id="join"></a>

We are always looking for talented and motivated individuals to join our research team. Below are the opportunities currently available.

### Postdoctoral Researchers

**Position Description:**  
Postdoctoral researchers in COALAB lead independent research projects while collaborating with other lab members. Positions are typically 2-3 years with possibility of extension.

**Current Openings:**
1. **Computational Linguistics/NLP Postdoc** - Focus on multilingual language model evaluation
2. **Cognitive Science Postdoc** - Focus on bilingual language processing and executive function

**Requirements:**
- PhD in Linguistics, Computer Science, Psychology, Cognitive Science, or related field
- Strong publication record
- Experience with relevant research methods (computational modeling, experimental design, etc.)
- Excellent communication and collaboration skills

**Application Process:**  
Send the following to [positions@coalab.org](mailto:positions@coalab.org):
1. CV
2. Research statement (2-3 pages)
3. Two representative publications
4. Names and contact information for three references

### PhD Students

**Programs:** We accept PhD students through:
- Department of Linguistics
- Department of Computer Science  
- Department of Psychology
- Cognitive Science Program

**Application Timeline:**
- **Application deadline:** December 15 (for fall admission)
- **Interviews:** January-February
- **Decisions:** March-April

**Funding:** All PhD students receive full funding (tuition + stipend) through research assistantships, teaching assistantships, or fellowships.

**How to Apply:**
1. Apply through the relevant department's graduate program
2. Mention your interest in working with COALAB in your statement of purpose
3. Contact Dr. Peter Awe to discuss research fit before applying

### Master's Students

**Opportunities:** Master's students can join the lab through:
- Research assistantships
- Thesis projects
- Course-based projects

**Current MSc/MA Programs:**
- MSc in Computational Linguistics
- MA in Linguistics
- MSc in Cognitive Science
- MSc in Computer Science

**Contact:** Interested master's students should email the relevant lab member with their CV and a brief description of research interests.

### Undergraduate Research Assistants

**Opportunities:** We regularly hire undergraduate research assistants for:
- Data collection and annotation
- Programming and software development
- Literature reviews
- Experimental assistance

**Requirements:**
- Strong academic record
- Interest in language research
- Relevant coursework (linguistics, computer science, psychology, etc.)
- Minimum 10 hours/week commitment

**Application:** Send your CV and transcript to [undergrad@coalab.org](mailto:undergrad@coalab.org)

### Visiting Scholars & Collaborators

We welcome visiting scholars and research collaborators from other institutions. Please contact Dr. Peter Awe to discuss possibilities.

## Contact Form

Have a question or want to get in touch? Use the form below:

<form id="contact-form" class="mt-4">
  <div class="row">
    <div class="col-md-6 mb-3">
      <label for="contact-name" class="form-label">Name *</label>
      <input type="text" class="form-control" id="contact-name" placeholder="Your Name" required>
    </div>
    <div class="col-md-6 mb-3">
      <label for="contact-email" class="form-label">Email Address *</label>
      <input type="email" class="form-control" id="contact-email" placeholder="name@example.com" required>
    </div>
  </div>
  
  <div class="mb-3">
    <label for="contact-affiliation" class="form-label">Affiliation</label>
    <input type="text" class="form-control" id="contact-affiliation" placeholder="University, Company, etc.">
  </div>
  
  <div class="mb-3">
    <label for="contact-subject" class="form-label">Subject *</label>
    <select class="form-select" id="contact-subject" required>
      <option value="" selected disabled>Select a subject</option>
      <option value="general">General Inquiry</option>
      <option value="collaboration">Research Collaboration</option>
      <option value="postdoc">Postdoctoral Position</option>
      <option value="phd">PhD Program</option>
      <option value="masters">Master's Program</option>
      <option value="undergrad">Undergraduate Research</option>
      <option value="visiting">Visiting Scholar</option>
      <option value="media">Media Inquiry</option>
      <option value="other">Other</option>
    </select>
  </div>
  
  <div class="mb-3">
    <label for="contact-message" class="form-label">Message *</label>
    <textarea class="form-control" id="contact-message" rows="5" placeholder="Your message..." required></textarea>
  </div>
  
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="contact-newsletter">
    <label class="form-check-label" for="contact-newsletter">Subscribe to our quarterly newsletter</label>
  </div>
  
  <button type="submit" class="btn btn-primary">Send Message</button>
</form>

<script>
document.getElementById('contact-form').addEventListener('submit', function(e) {
  e.preventDefault();
  
  // Simple validation
  let isValid = true;
  const requiredFields = this.querySelectorAll('[required]');
  
  requiredFields.forEach(field => {
    if (!field.value.trim()) {
      field.classList.add('is-invalid');
      isValid = false;
    } else {
      field.classList.remove('is-invalid');
    }
  });
  
  if (isValid) {
    const submitBtn = this.querySelector('button[type="submit"]');
    const originalText = submitBtn.textContent;
    
    submitBtn.textContent = 'Sending...';
    submitBtn.disabled = true;
    
    // Simulate form submission
    setTimeout(() => {
      alert('Thank you for your message! We will get back to you soon.');
      this.reset();
      submitBtn.textContent = originalText;
      submitBtn.disabled = false;
    }, 1500);
  }
});
</script>

## Directions & Parking

### Getting Here
**By Public Transit:**  
Take the subway to University Station, then walk 10 minutes north to the Science Building.

**By Car:**  
Visitor parking is available in Lot P5. Daily parking passes can be purchased at the parking office.

**Accessibility:**  
The Science Building is fully accessible. Please contact us in advance if you require any accommodations.

### Lab Tours
Interested in visiting the lab? We offer tours by appointment. Please contact us at least one week in advance to schedule a visit.

## Mailing List

Stay updated with lab news, events, and opportunities:

- **Quarterly Newsletter:** [Subscribe here](#newsletter-form)
- **Announcement List:** For immediate updates on talks and events
- **Research Discussion List:** For lab members and collaborators

## Social Media

- **Twitter/X:** [@COALAB_Research](https://twitter.com/COALAB_Research)
- **GitHub:** [github.com/coalab](https://github.com/coalab)
- **Google Scholar:** [COALAB Profile](https://scholar.google.com/citations?user=coalab)

## Partnerships & Collaboration

We actively seek collaborations with:
- Academic researchers in related fields
- Industry partners for applied research
- Clinical practitioners for translational work
- Community organizations for outreach

If you're interested in collaborating, please contact Dr. Peter Awe directly with a brief description of your proposed collaboration.

---

*Last updated: January 2025*
