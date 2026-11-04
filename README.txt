upGrad UPI checkout prototype, V11 (the final direction): coupon option B, and on phones the Full
details header

index.html   V11, the final direction (described below): the offer link names no centre or
             batch; the learner picks the learning centre on the details page. Step 1 and 2 are
             the offer page and the details (with the OTP); step 3 is the payment page (V1's
             page, Figma 73:3744, with the payment-options tabs from 78:5054), a desktop layout
             (1512px wide) with upGrad's mobile checkout on phones.

Open index.html in a browser. The "Scenario" menu at the top jumps to any state: logged in
or out, last hour, under 10 minutes left, an offer that ends while the page is open, the
payment page's review (and an offer that ends on the payment page), and the other link states. On the payment page, the upGrad logo
starts the flow again.

Text is set in upGrad's Circular, embedded in the page; Circular has no ₹ sign, so that
one glyph comes from Inter (online) or a system font (offline). Circular is licensed to
upGrad: keep this file internal. The UPI QR is a sample and cannot take a payment.

For user testing, add ?test to the link (index.html?test): no Scenario bar, no version switch and
no prototype notes; it opens on V11, option B, at the offer page, with the Full header on
phones. The code hint reads "For this test, enter any 6 digits as the code.", and Proceed to
Pay ends with "That's the end of this test. No payment is taken."

On the payment page, the switch in the bottom-left corner also has Restart (that page has no
Scenario bar), and the upGrad logo starts the flow again every time it is pressed.

Preview: V11 only, with coupon option B and, on phones, the details page's Full header. The
other options and versions are dropped: coupon options A and C, the phone headers Minimal, Medium
and Full 2, and the trial copies V12 to V15. Any older link (?v=9, ?v=10a to ?v=10c, ?v=11a,
?v=11c, ?v=12 to ?v=15, any &pd=) opens this one and is rewritten to say so. The switch in the
bottom-left corner keeps V11 and Replay (Restart on the payment page). What V11 builds on
(V10, V9, then V5 to V8) is described after it.

V11          V10, the final direction: the link names no centre or batch, and the learner picks
             the learning centre on the details page. Coupon option B (A and C are dropped).
             1. Offer page: the coupon has no centre or batch start, and the course's name drops
                the centre ("Advance Certificate in Digital Marketing"). No duration either (the
                details page shows it, under the centre picked), so one dashed line parts the
                course from the price.
                The saving reads "Save ₹10,000" (it was "You save ₹10,000").
                The prices, the ₹5,000 block and the countdown are as in V10, except that in
                option B the countdown line is centred on the coupon (here and on the details
                page): one short line between the full-width box and the full-width button. (A and
                C keep it at the left edge, with their left-set prices.) On a 360px phone the line
                is set a little tighter so it stays on one line; under 340px "9:00 PM today" takes
                a line of its own.
                The coupon (here and on the details page) keeps one spacing rule: each section has
                the same inset as the coupon's sides (24px, 20px on phones) above and below each
                dashed line, the price's parts are 16px apart, and the button has as much space
                under it (to the top of the scallops) as over it. Also once the offer has ended.
             2. Details, logged in or out (logged-in learners no longer skip it):
                - "Learning centre" is the first field: a search box ("Search by city or area").
                  Typing narrows the centres with a batch coming up, from the start of any word
                  ("ba" or "Bengaluru" finds the Bangalore centres; "hsr", "sector" or "34" work
                  too), with the letters typed in bold; a tap or the chevron opens the whole list,
                  A to Z ("Bangalore – HSR Layout"). Arrow keys move, Enter picks, Escape closes.
                  No match says "No centre matches "…". Try a city or an area." Leaving the box
                  with text that names no centre puts back the centre picked (or empties it).
                - Once one is picked, its batch start and duration show just under the list
                  ("Batch starts Sat, Nov 21, 2026", "Duration 4 months"), not in the coupon on
                  the right, which keeps to the price.
                - It is required: Continue without one says "Select the learning centre you'll
                  attend." under it and moves there.
                - Continue, until the details are in, is the brand red at 60% opacity (down 40%),
                  white label (it was a washed-out pink, #F7A8AE); full strength once they are in.
                  It has no line under it (no "Fill in your name, email and mobile to continue",
                  no "We'll send a code to verify your mobile", which the mobile's own help
                  already says). It waits for the centre, name, email and mobile: pressed before
                  they are all in, it does not go on: it shows what is missing under each field,
                  moves to the first and shakes them.
                - Phones, the pinned header: Full (Minimal, Medium and Full 2 were tried and are
                  dropped). The whole header is pinned at the top, the course's name included.
                  There is no title row ("‹ Your Details"; the card under it is titled "Your
                  details"): back is at the start of the course row, so the room is the offer's.
                  Full: the course, then the offer, "Course fee ₹90,000 ₹1,00,000" with "You
                  save ₹10,000", over a box split in two, "Pay now ₹5,000" (the one strong
                  number) and "Remaining ₹85,000" (grey, regular, smaller), then the strip at the
                  foot (the countdown and when the offer ends, "9:00 PM today"); 184px. Once the
                  page is scrolled, the course fee line folds away (about 156px pinned); back at
                  the top, it is back.
                  Once the offer has ended, the extra lines go (the strip shows the full price).
                - Logged in, the name, email and mobile come filled in from the account and can
                  be edited ("Filled in from your upGrad account. You can edit them."; the heading
                  says "Confirm your details."). The mobile shows "Verified": kept, Continue goes
                  straight to checkout; changed, the line says "We'll send a code to verify it."
                  and Continue asks for the code.
             3. Checkout: no centre step (it was picked on the details page). The course card names
                the centre and its batch ("Pune – Kothrud · 4 months · Starts Dec 5, 2026"); Back
                returns to the details page to change it. The confirmation shows the centre and
                its batch start, and the balance is due before that date.
                Choosing how to pay, the ₹5,000 that locks the offer leads, and what remains
                follows it, small (the Summary beside the options already shows how the fee comes
                to ₹90,000, so the card doesn't repeat it). On desktop the course card's price
                column reads "Minimum to lock your offer", ₹5,000 large, then "Remaining ₹85,000
                later" under it, smaller; Reserve a Seat (the ₹5,000 option) is open first, not
                Recommended. On phones the pinned strip reads "₹5,000 minimum to lock" first and
                "Remaining ₹85,000 later" after it, smaller. On the
                review (an option is picked, maybe the full fee), for a reserved seat's balance,
                and when the page opens after the offer has ended, the card shows the course fee
                as before. (A learner who reached the page while the offer was live keeps the
                offer price, so the ₹5,000 stays.)
                On phones the billing postal code / PIN code is now shown too, in a card over
                "Choose a payment option" (desktop has it as step 1): filled in, editable, with
                the place it finds under it. It is the same code as desktop's field. Tapping an
                option with a code missing or wrong says so under it and moves to it.
             Journey progress: one bar from the offer page to the payment, at the top of
             the flow's pages (they have no top bar: no logo, "Secure checkout" or Log in) and
             under the payment page's header. A light track shows the
             whole way; the fill (green to blue) shows how far the learner has come: offer 12.5%,
             details 37.5%, payment options 62.5%, review 87.5%, paid 100%, so it never goes
             back between pages (before V11 it went from 37.5% on the details page to 15% on the
             payment page). Plain: no glow, and no marker at the fill's end. No bar on the link
             states with nothing to pay. On phones it sits along the very top of every page, full
             width and pinned, as on the offer page.
             The centres are the 12 on the centre list with a proper centre name (city and
             locality); the 16 listed by city alone (Bhubaneswar, Gurugram, Jaipur, Bhilwara,
             Dehradun, Haldwani, the second Kolkata centre, Coimbatore, Nagercoil, Belagavi,
             Mangalore, Chhatrapati Sambhaji Nagar, Bhopal, Jabalpur, Raipur, Rajkot) are left
             out. Their batch dates are samples (Nov 21 to Dec 12, 2026); Bangalore – Jayanagar is
             given no batch coming up, to show how such a centre is left out, so the list shows
             11. Every centre has the course's 4 months. Opened straight from the Scenario menu,
             the payment page shows Bangalore – Marathahalli. Paying the balance
             of a reserved seat asks for no centre.

(V12 to V15, copies of V11 with new offer and details pages, were tried and dropped; their notes
are in this branch's history.)

What V11 builds on (no longer in the switch):

V10          V9, and the coupon leads with the ₹5,000 that locks the offer. The
             course price (₹90,000, ₹1,00,000 struck) sits under it, small, with no strike or
             price animation. The offer page's button reads "Lock offer for ₹5,000", and on phones
             the details page's strip reads "Lock for ₹5,000" in place of the price. Three options
             (A, B, C beside V10 in the switch):
             A. "Course fee ₹90,000" (₹1,00,000 struck) with "You save ₹10,000" at the right,
                then "Pay now to lock your offer", ₹5,000 large, and "Remaining amount ₹85,000".
             B. Kept short: "Course fee ₹90,000" (₹1,00,000 struck) with "You save
                ₹10,000" at the right, as in V9, then a box with "Pay now ₹5,000" (large) over
                "Remaining amount ₹85,000" (no date, so the balance does not read as a deadline).
             C. The two payments as steps: "Course fee ₹90,000" with "You save ₹10,000" at the
                right, then Pay now, ₹5,000 (large, a red dot; "Locks your course fee") and
                Remaining amount, ₹85,000.
             All three use B's words (Course fee, Pay now, Remaining amount) and name no date for
             the balance.
             On desktop the details page's coupon is 400px wide (360px before), so the course fee
             line fits on one line, and the details card has more room (36px padding, 28px
             between fields, 56px fields), so the two cards are closer in height.
             The details page has no prototype note under the mobile field (V9's names the test
             numbers; they still work, and the Scenario menu has both states).
             The payment page is V8's, not V9's Microsoft layout: Reserve a Seat (pay at least
             ₹5,000, the amount can be raised), Recommended, Pocket-Friendly and Other options;
             Proceed to Pay ends the prototype there, as in V8.
             Once the offer has ended the coupon is V9's. The rest of the flow is V9's.

V9           V7, and the offer link takes the block amount only, ₹5,000 (never more):
             1. Offer page: the button reads "Reserve seat for ₹5,000", with nothing under
                it; no way to pay in full here.
             2. Details: the form is the same, the button reads "Continue to pay
                ₹5,000". After the OTP, 90000 00000 (block paid) opens
                "Your seat is already reserved"; 90000 00001 (paid in full) opens "You're
                already enrolled".
             3. Payment page (the offer price locked), as upGrad's checkout for Microsoft courses:
                "Welcome <name>", the course card (logo, UPGRAD EDUCATION PVT LTD, the course),
                then Payment Methods: UPI, Credit Card, Debit Card and Net Banking on the left (the
                picked one pink, with a chevron), its panel beside them (UPI: "Scan QR code", two
                steps, the apps, a blurred QR with Show QR Code; a card form; banks). On the right
                rail, Billing details (state and PIN code, the pencil edits it) and the Price
                breakup (course fee, offer, course price, balance ₹85,000; Pay now ₹5,000) with
                "Proceed to Pay ₹5,000". No EMI, no amount to enter. On phones the course is in the
                pinned header, the cards stack, and the button stays at the foot of the screen.
             4. Confirmation: "Your seat is locked at ₹90,000", what was paid and the balance
                row; Pay balance opens the regular payment page (all options) for ₹85,000.
             5. "Your seat is already reserved" (Scenario: Seat already reserved): when the block
                was paid and the balance (₹85,000) is due before Oct 31; "Pay remaining ₹85,000"
                opens the regular payment page. "You're already enrolled" stays for learners who
                paid in full.
             "Link not open yet" and a link opened after the offer ended keep "Pay full price now"
             and the full-price checkout, where Reserve a Seat is also exactly ₹5,000 ("Pay INR
             5,000", no amount to enter).

Before that, V5 to V8:
V5           V9 with a trimmed coupon: no heading over it ("An offer from upGrad
             Marathahalli."), no "Your course" line, and the saving ("You save ₹10,000") on the
             price's line, at the coupon's right edge. On phones the details page shows the
             coupon first, then the details card.
             On the offer page the coupon prints out of a printer, as in the references: a
             light housing with a recessed window; the coupon comes out from under the window's
             back edge (the rollers), lies over the housing's front and hangs below. The print
             follows the Dribbble interaction: a coupon already out is pulled back in, then it
             creeps out a fifth of the way with a small jitter, then glides out and slows to
             rest (about 1.5s). The coupon gets a scalloped bottom edge; its top corners are
             near-square on the offer page and rounded on the details page. It prints on
             opening, on a scenario or Restart and on Replay (in the switch), not when coming
             back from the details; with reduced motion it is simply there.
             The offer page has no header (logo, "Secure checkout", Log in, progress bar); it
             comes in from the details page on.
             As the coupon lands, the price reveals itself one step at a time (about 1.6s): a
             line strikes through ₹1,00,000, shown as the price; it moves up into its place
             beside "Course fee"; ₹90,000 comes in where it stood, with the countdown under it
             at the same moment and with the same motion; then "You save ₹10,000" pops in.
             Only while the offer is live; not with reduced motion.
             The price is labelled "Course fee" (as on the payment page), beside the struck
             list price while the offer is live, and alone above the full price once it ends.
             The offer's countdown ("Offer ends in 17:44:12 · 9:00 PM today") sits under the
             final price, so it reads as the price's deadline: what it costs, what you save,
             until when. On the coupon (offer and details pages) and on the payment page's
             course card. Its clock ticks: the second hand steps on each second, a full turn in
             12 seconds (not with reduced motion).
             The time always shows seconds (08:05:42, not 8h 5m), a size up and bold, in every
             live state (logged out, logged in, the last hour, the last 10 minutes); in the last
             minute it goes a size up again with a soft beat each second (no beat with reduced
             motion). Also on the payment page.
             Once the offer ends, the coupon says "Offer ended at 9:00 PM" where the countdown
             was. The payment page's summary shows the Offer row as "INR -10,000" struck through
             (a brand-red line, tilted a little), with "Offer ended at 3:05 PM" under it; that is
             the only place the payment page says it (the course card does not repeat it).
             The offer page's button says "Claim now" (it was "Apply Offer").
             The details page's heading says "Almost there. Add your details." (it was "Almost
             there. Who is joining?").
             The payment page's course card has no "↓10%" before the struck list price.
             The coupon's course name is a little larger: 17px (16px on phones; 15px in the
             phone details summary).
             On phones, the details page shows the coupon as a short summary (the countdown, the
             course and the price; no centre, batch start or duration) so the name, email and
             mobile fields come into view.
             On the details page, Continue waits for the name, email and mobile to pass the
             page's checks; meanwhile the line under it says what to fill in. Every disabled
             button (Continue, Verify, "Verifying…", the payment page's Next) is #F15663 with its
             label in full white. It stays clickable: pressed before the details are in, it
             shows the errors under what is missing (with a small shake) and moves to the
             first. The OTP sheet's Verify gets the same until all six digits are in: pressed
             early, it says "Enter the 6-digit code we sent to your mobile." (or "Enter all 6
             digits of the code."), and the code boxes shake.
             A logged-out learner's billing code is filled in from their location: 560037,
             Marathahalli, Bengaluru (editable).

V6           V5, and the payment page's first step reads "1. Billing Postal Code / PIN Code" (most
             learners know it as a PIN code; its messages say PIN code too). Its field lines up
             with the payment cards' right column (the same left edge and width as the second
             card), and the place found for the code ("Bengaluru, Karnataka") sits under it,
             right-aligned to the same edge as the field and the cards.
             The code is filled in from the learner's location when they have none on file
             (logged out), as in V5.

V7           V6, and the offer does not run out on the payment page: a learner who gets there while
             the offer is live keeps the offer price (₹90,000) for that visit, however close to the
             end they came, through the options and the review. The payment page shows no timer: on
             desktop the course card shows the price and the saving; on phones the pinned strip
             shows the price, and "You save ₹10,000" where the countdown was. The offer and details pages keep their
             countdown, and a learner who reaches checkout after the offer has ended pays the full
             price, as before. (Try "Offer ends in 10 seconds" under Payment page.)

V8           V7, and the offer page's button reads "Reserve seat for ₹5,000" (it was "Claim now").
             To match it, the payment page reserves the seat for ₹5,000: "Pay minimum INR 5,000
             now" under Reserve a Seat, an amount between INR 5,000 and the price, and INR 5,000
             paying now when a method is picked on phones. V5 to V7 keep INR 10,000.

On phones (up to 860px wide), the payment page (V5 to V7) is upGrad's mobile checkout (Figma
94:6801): a "Payment Options" header with Back and the progress that also carries, pinned however
far the options are scrolled, the course (logo, name, and "Marathahalli, Bengaluru · Starts Oct 31 ·
4 months", one line down to 360px) and a thin strip with the offer's countdown and price (once the offer ends, when it
ended and the full price), then "Choose a payment option":
Reserve a Seat (pay at least INR 10,000 now by card, net banking or UPI), Recommended (Credit Card
EMI over 24 months; No Cost Cardless EMI over 6 months with Propelld, Fibe or Northernarc),
Pocket-Friendly (Standard EMI at 18%) and Other options (the full amount by card or net banking),
and Back to Top. The details page uses the same header on phones ("Your Details", with Back to
the offer) in place of its heading ("Almost there. Add your details.", kept for screen readers),
and in place of the coupon its header carries the course (logo and name) and a thin strip with
the offer's countdown and price ("Offer ends in 00:59:12" and "₹90,000 ₹1,00,000"), all pinned to the
top however far the form is scrolled. The amounts follow this course's price (INR 90,000 while the offer is live, INR
1,00,000 after), not the frame's sample course. Picking an option opens the page's review, as on
the desktop page (the review itself is the desktop page). From 861px the payment page is as
before.

The "Offer ends in 10 seconds" scenarios (offer page, payment page, review) end the offer 10 seconds
after they open, to see the end without a long wait (they were 30 seconds).
