document.addEventListener('DOMContentLoaded', () => {
  const testimonials = [
    {
      text: "Taniya was absolutely amazing! Her energy lit up the entire event.",
      author: "Rohit Sharma"
    },
    {
      text: "Professional, charismatic, and engaging. Highly recommended!",
      author: "Anjali Mehta"
    },
    {
      text: "She made our wedding unforgettable. Thank you, Taniya!",
      author: "Karan Patel"
    }
  ];

  let currentIndex = 0;
  const testimonialText = document.getElementById('testimonial-text');
  const testimonialAuthor = document.getElementById('testimonial-author');
  const prevBtn = document.getElementById('prev-testimonial');
  const nextBtn = document.getElementById('next-testimonial');

  function updateTestimonial(index) {
    testimonialText.textContent = testimonials[index].text;
    testimonialAuthor.textContent = testimonials[index].author;
  }

  prevBtn.addEventListener('click', () => {
    currentIndex = (currentIndex - 1 + testimonials.length) % testimonials.length;
    updateTestimonial(currentIndex);
  });

  nextBtn.addEventListener('click', () => {
    currentIndex = (currentIndex + 1) % testimonials.length;
    updateTestimonial(currentIndex);
  });

  // Initialize with the first testimonial
  updateTestimonial(currentIndex);
});
