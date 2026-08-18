<?php

$firstname = $_POST['firstname'];
$lastname = $_POST['lastname'];
$email = $_POST['email'];
$verify_email = $_POST['verify_email'];
$phone = $_POST['phone'];
$reservation_date = $_POST['reservation_date'];
$subject = $_POST['subject'];
$message = $_POST['message'];

if ($email != $verify_email) {
    die("Email addresses do not match.");
}

$to = "your_email@example.com"; // Replace with your email

$email_subject = "Contact Form Submission";

$email_body = "Name: $firstname $lastname\n";
$email_body .= "Email: $email\n";
$email_body .= "Phone: $phone\n";
$email_body .= "Reservation Date: $reservation_date\n";
$email_body .= "Subject: $subject\n\n";
$email_body .= "Message:\n$message";

$headers = "From: $email";

mail($to, $email_subject, $email_body, $headers);

echo "<h2>Thank you! Your message has been sent.</h2>";

?>