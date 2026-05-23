# WhatsApp Group Login

A simple web-based login interface to access WhatsApp group invitations.

## Features

- Clean and modern login UI with WhatsApp branding
- Responsive design
- Easy group link access after authentication

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/davismaiba25-rgb/what-sapp.-login.git
cd what-sapp.-login
```

### 2. Configure Environment Variables

Create a `.env` file in the root directory:
```
WHATSAPP_GROUP_LINK=https://chat.whatsapp.com/YOUR_GROUP_INVITE_CODE
ADMIN_USERNAME=your_admin_username
ADMIN_PASSWORD=your_secure_password
```

### 3. Run Locally

Open `index.html` in your web browser, or use a local server:
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (if you have http-server installed)
http-server
```

Visit `http://localhost:8000` in your browser.

## Important Security Notes

⚠️ **This current implementation is for demonstration purposes only.**

### Security Considerations:

1. **Client-Side Authentication**: The current implementation validates credentials in the browser, which is **not secure** for production use.

2. **Never commit credentials** to your repository. Use environment variables or a backend server instead.

3. **For Production**:
   - Implement server-side authentication
   - Use proper password hashing (bcrypt, argon2, etc.)
   - Store credentials securely in a database
   - Use HTTPS only
   - Implement rate limiting to prevent brute force attacks
   - Consider using OAuth or other authentication providers

## Getting Your WhatsApp Group Invite Link

1. Open WhatsApp
2. Go to the group you want to share
3. Tap the group name at the top
4. Scroll down and select "Invite via link"
5. Tap "Copy link"
6. Paste the link in your `.env` file

## Usage

- Username: `admin` (default - change this!)
- Password: `1234` (default - change this!)

## Future Improvements

- [ ] Backend server implementation
- [ ] Database integration
- [ ] User registration system
- [ ] Password reset functionality
- [ ] Rate limiting
- [ ] HTTPS support
- [ ] Session management

## License

MIT

## Support

For issues or questions, please open a GitHub issue.
