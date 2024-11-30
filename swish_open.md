Försöker öppna Swish-appen...

<script>
  document.addEventListener("DOMContentLoaded", function startSwish() {
        const payload = {
            "version": 1,
            "payee": {
                "value": "1232295269"
            },
            "message": {
                "value": "People For Future Umeå",
                "editable": false
            }
        };

        const encodedPayload = encodeURIComponent(JSON.stringify(payload));
        const callbackUrl = "https://pffumea.se/swish_thanks"; // Din callback-URL
        const encodedCallbackURL = encodeURIComponent(callbackUrl);

        const swishUrl = `swish://payment?data=${encodedPayload}&callbackurl=${encodedCallbackURL}`;

        // Försök växla till Swish-appen
        window.location.href = swishUrl;
    });
</script>
