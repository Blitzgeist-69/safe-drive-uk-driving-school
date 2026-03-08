# Safe Drive UK Driving School - Testing Documentation

**Testing Strategy**
The testing strategy for Safe Drive UK is **user-story driven** and follows a **mobile-first** approach.

**Core principles:**

- Every feature is tested against its Acceptance Criteria before being marked complete.
- Testing is performed on real devices and browser DevTools to simulate real users.
- Accessibility and performance are treated as equally important as visual design.
- All testing is documented with evidence (screenshots saved in a `/testing-screenshots` folder in the repo).
- Bugs are logged immediately and re-tested after fixes.

**Testing types used:**

- Manual functional testing
- Responsiveness testing
- Accessibility & SEO checks
- HTML/CSS validation
- Cross-browser compatibility
- User-story validation

## Testing Plan

**Phase 1 – Unit/Feature Testing** (during development)  
Test each component (navbar, hero, cards, form, modals) as it is built.

**Phase 2 – User Story Validation**  
Go through every Must-Have, Should-Have and Could-Have user story.

**Phase 3 – Full Site Validation** on deployed site.

- Run all validators and Lighthouse
- Test on real devices
- Document bugs and fixes

**Tools used:**

- Chrome DevTools inc Lighthouse
- Firefox
- Microsoft Edge
- W3C HTML & CSS Validators
- WAVE Accessibility Tool
- Real devices: Windows 11 Desktop, Windows 10 Laptop, Samsung Galaxy A55 phone, Samsung S4 Galaxy Tab

**Test Environment:**

- Operating System: Windows 11 / 10, Android 10 / 16
- Browser versions: Chrome 142 / 145, Firefox 147, Edge 145,

**Validators**

- HTML: W3C Markup Validation – **TBC**
- CSS: W3C CSS Validation – **TBC**

**Lighthouse (Chrome DevTools) – Desktop and Mobile**

- Performance: **TBC**
- Accessibility: **TBC**
- Best Practices: **TBC**
- SEO: **TBC**

**Browser & Device Testing**

- Chrome, Firefox, Edge, Safari (desktop)
- iPhone, iPad, Samsung Galaxy (via Chrome DevTools)
- Real phone testing on Android

**User Story Testing**
| User Story | Test Performed | Result | Evidence |  
|----------------------|------------------------|---------------|---------------|  
| | | | |  
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |

**Bugs Encountered & Fixed**

| Expected Outcome                                                                                                                             | Actual Outcome                                                                       | Bug Cause                                                                                      | Bug Fix                                                                                                                                                                                                                | Evidence of fix                                                                                  |
| -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| Success page footer title is consistent with other pages                                                                                     | [![Bug 1](./assets/screenshots/bug_1_sduk.png)](./assets/screenshots/bug_1_sduk.png) | Different h tag level. h3 on index.html and booking.html.  h2 on success.html                  | Amend success.html to h3                                                                                                                                                                                               | [![Bug 1 Fix](./assets/screenshots/bug_1_fix_sduk.png)](./assets/screenshots/bug_1_fix_sduk.png) |
| Contact Details – first line of address stays on single line for all screen widths                                                           | [![Bug 2](./assets/screenshots/bug_2_sduk.png)](./assets/screenshots/bug_2_sduk.png) | Address was in a narrow column col-md-2 and was wrapping in certain contexts                   | Added span class="text-nowrap" to first line of address on all footers                                                                                                                                                 | [![Bug 2 Fix](./assets/screenshots/bug_2_fix_sduk.png)](./assets/screenshots/bug_2_fix_sduk.png) |
| social links in footer do not show underlines                                                                                                | [![Bug 3](./assets/screenshots/bug_3_sduk.png)](./assets/screenshots/bug_3_sduk.png) | text decoration underline is partly displayed on social links on success.html                  | Add CSS .social-link a {text-decoration: none:}                                                                                                                                                                        | [![Bug 3 Fix](./assets/screenshots/bug_3_fix_sduk.png)](./assets/screenshots/bug_3_fix_sduk.png) |
| The text is clear and reads well                                                                                                             | [![Bug 4](./assets/screenshots/bug_4_sduk.png)](./assets/screenshots/bug_4_sduk.png) | Text included a duplication of "Thank you" that was not required                               | Change first p to h2 and add classes 'small' and 'fw-bold'. Amended text.                                                                                                                                              | [![Bug 4 Fix](./assets/screenshots/bug_4_fix_sduk.png)](./assets/screenshots/bug_4_fix_sduk.png) |
| The hero does not extend to full width as shown in wireframe and text and CTA appear on screen without the need to scroll to se them         | [![Bug 5](./assets/screenshots/bug_5_sduk.png)](./assets/screenshots/bug_5_sduk.png) | Hero image did not have CSS styling to control width                                           | Add CSS .hero picture {<br>    max-width: 88%;<br>    margin: 0 auto;<br>    display: block;<br>}.                                                                                                                     | [![Bug 5 Fix](./assets/screenshots/bug_5_fix_sduk.png)](./assets/screenshots/bug_5_fix_sduk.png) |
| The hero does not extend to full width as shown in wireframe and text and Return Home appear on screen without the need to scroll to se them | [![Bug 6](./assets/screenshots/bug_6_sduk.png)](./assets/screenshots/bug_6_sduk.png) | Hero image did not have CSS styling to control width                                           | Add CSS .hero picture {<br>    max-width: 88%;<br>    margin: 0 auto;<br>    display: block;<br>} and change mt-3 to mt-2 on Return to home button. Remove unused #hero-passed                                         | [![Bug 6 Fix](./assets/screenshots/bug_6_fix_sduk.png)](./assets/screenshots/bug_6_fix_sduk.png) |
| There is clear indication that the booking form has more fields to complete and the Submit button is available                               | [![Bug 7](./assets/screenshots/bug_7_sduk.png)](./assets/screenshots/bug_7_sduk.png) | No visual indication that form continues below visible portion of screen especially on desktop | Add card wrapper to form and CSS styling. .booking-form {<br>    background-color: var(--primary-green);<br>    padding: 1rem;<br>    color: var(--bg-light);<br>    box-shadow: 0 0 0 4px var(--secondary-navy);<br>} | [![Bug 7 Fix](./assets/screenshots/bug_7_fix_sduk.png)](./assets/screenshots/bug_7_fix_sduk.png) |
| The service card badges show consistent alignment                                                                                            | [![Bug 8](./assets/screenshots/bug_8_sduk.png)](./assets/screenshots/bug_8_sduk.png) | Inconsistent margins on Services cards                                                         | Remove inconsistent margins on Services cards and add margin-top: auto; to CSS .card .badge                                                                                                                            | [![Bug 8 Fix](./assets/screenshots/bug_8_fix_sduk.png)](./assets/screenshots/bug_8_fix_sduk.png) |

**Known Issues**

**TBC**

## Future Improvements

- Availability calendar
- Google Maps embed

## Conclusion

**TBC**

**Ready for deployment and submission.**
