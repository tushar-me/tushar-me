
<h1 align="center">Hi 👋, I'm Tushar Imran</h1>
<h3 align="center">Full Stack Web Developer</h3>


<p align="left"> <img src="https://komarev.com/ghpvc/?username=tushar-me&label=Profile%20views&color=0e75b6&style=flat" alt="tushar-me" /> </p>

- 💬 Ask me about **Web Development**
- 📫 How to reach me **tusharimran.dev@gmail.com**
- 👨‍💻 All of my projects are available at [https://tusharimran.site/](https://tusharimran.site/)


<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://fb.com/tusharimran.online" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="tusharimran.online" height="30" width="40" /></a>
<a href="https://instagram.com/tushar.imran.me" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="tushar.imran.me" height="30" width="40" /></a>
<a href="https://stackoverflow.com/users/21828294" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/stack-overflow.svg" alt="21828294" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://laravel.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/laravel/laravel-plain-wordmark.svg" alt="laravel" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://www.php.net" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"/> </a> <a href="https://sass-lang.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sass/sass-original.svg" alt="sass" width="40" height="40"/> </a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="40" height="40"/> </a> </p>

<p align="left">
	<img width="48%" src="https://github-readme-streak-stats.herokuapp.com/?user=tushar-me&theme=github" />
</p>

### GitHub Profile Summary Card
<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=tushar-me&theme=github"/>
</p>

### Top Commits
<p align="center">
	<img width="48%" src="http://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=tushar-me&theme=github&utcOffset=8" />
</p>

### Top Languages
<p align="center">
	<img width="48%" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=tushar-me&theme=github" />
	<img width="48%" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=tushar-me&theme=github" />
</p>


<div style="background-color: black; color: white; padding: 10px;">
```php
public function storeProduct(ProductRequest $req)
{

    $data = $req->validated();
    $data['user_id'] = Auth::id();
    $product = Product::create($data);


    $images = request()->images;

    $imageData = [];
    foreach( $images as $image){
        $imageData[] = [
            'url' => '/storage/'.$image['file']->store('uploads', 'public'),
            'product_id' => $product->id
        ];
    }
    Image::insert($imageData);
    return to_route('product.all');
}

```
</div>
