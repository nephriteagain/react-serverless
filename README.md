#### Netlify TOML for create-react-app

[build]

- command = 'npm run build'
- publish = '/build'
- functions = './functions'

[[redirects]]

- from = '/api/\*'
- to = '/.netlify/functions/:splat'
- status = 200

[[redirects]]

- from = '/\*'
- to = '/index.html'
- status = 200

#### build Command

"build": "CI= react-scripts build"
#   r e a c t - s e r v e r l e s s  
 