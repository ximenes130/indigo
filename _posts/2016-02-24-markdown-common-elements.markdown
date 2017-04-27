---
title: "Elementos comuns do Markdown"
layout: post
date: 2017-04-24 17:44
image: /assets/images/markdown.jpg
headerImage: false
tag:
- markdown
- elements
star: true
category: blog
author: wendelribi
description: Resumo de markdown com diferentes opções
---

## Resumo:

Você pode escolher como item para ver como aplicar em markdown.

### Elementos Comum
- [Formatação básica](# formatação básica)
- [Cabeçalhos](# cabeçalhos)
- [Listas](# listas)
- [Modificadores de parágrafo](# parágrafo-modificadores)
- [Urls](# urls)
- [Regra Horizontal](# regra horizontal)
- [Imagens](# imagens)
- [Código](# código)
---

## Formatação básica

Esta nota ** demonstra ** algum do que [Markdown] [1] é * capaz de fazer *.

E é assim que se faz.

{% highlight html%}
Esta nota ** demonstra ** algum do que [Markdown] [algum / link] é * capaz de fazer *.
{% endhighlight %}

---
##Cabeçalhos

Existem seis níveis de títulos. Eles correspondem aos seis níveis de cabeçalhos HTML. Você já deve ter notado eles já na página. Cada nível abaixo usa mais um caractere de hash. Mas estamos usando apenas 4 deles.

# Os cabeçalhos podem ser pequenos

## Os cabeçalhos podem ser pequenos

### Os cabeçalhos podem ser pequenos

#### Os cabeçalhos podem ser pequenos

{% highlight raw%}
# Heading
## Heading
### Título
#### Título
{% endhighlight %}

---

## Listas

### Lista ordenada

1. Item 1
2. Um segundo item
3. Nº 3

{% highlight raw%}
1. Item 1
2. Um segundo item
3. Número 3
{% endhighlight %}

### Lista desordenada

* Um item
* Outro item
* Ainda outro item
* E há mais ...

{% highlight raw%}
* Um item
* Outro item
* Ainda outro item
* E há mais ...
{% endhighlight %}

---

## Modificadores de parágrafo

### Citação

> Aqui está uma citação. O que isto deve ser auto-explicativo. As citações são automaticamente recuadas quando são usadas.

{% highlight raw%}
> Aqui está uma citação. O que isto deve ser auto-explicativo.
{% endhighlight raw%}

---

## URLs

Os URLs podem ser feitos de várias maneiras:

* Um link com nome para [Mark It Down] [3].
* Outro link com nome para [Mark It Down](http://markitdown.net/)
* Às vezes você só quer um URL como <http://markitdown.net/>.

{% highlight raw%}
* Um link com nome para [MarkItDown] [3].
* Outro link com nome para [MarkItDown](http://markitdown.net/)
* Às vezes você só quer um URL como <http://markitdown.net/>.{% endhighlight %}

---

## Regra horizontal

Uma regra horizontal é uma linha que atravessa o meio da página.
Às vezes é útil para quebrar as coisas.

{% highlight raw %}
---
{% endhighlight %}

---

## Imagens

Markdown também pode conter imagens. Preciso adicionar algo aqui algum dia.

{% highlight raw %}
![Markdowm Image][/image/url]
{% endhighlight %}

! [Imagem de Markdown] [6]

* Legenda da figura *?

{% highlight raw %}
![Markdowm Image][/image/url]
<figcaption class="caption">Foto do Homer</figcaption>
{% endhighlight %}

![Markdowm Image][6]
<figcaption class="caption">Foto do Homer</figcaption>

* Imagens maiores *?

{% highlight raw %}
![Markdowm Image][/image/url]{: class="bigger-image" }
{% endhighlight %}

![Markdowm Image][6]{: class="bigger-image" }

---

Código

Um exemplo de HTML:

{% highlight html %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Documento</title>
</head>
<body>
    <h1>Test</h1>
</body>
</html>
{% endhighlight %}

Um exemplo CSS:

{% highlight css %}
pre {
    padding: 10px;
    font-size: .8em;
    white-space: pre;
}

pre, table {
    width: 100%;
}

code, pre, tt {
    font-family: Monaco, Consolas, Inconsolata, monospace, sans-serif;
    background: rgba(0,0,0,.05);
}
{% endhighlight %}

Um exemplo JS:

{% highlight js %}
// Sticky Header
$(window).scroll(function() {

    if ($(window).scrollTop() > 900 && !$("body").hasClass('show-menu')) {
        $('#hamburguer__open').fadeOut('fast');
    } else if (!$("body").hasClass('show-menu')) {
        $('#hamburguer__open').fadeIn('fast');
    }

});
{% endhighlight %}

[1]: http://daringfireball.net/projects/markdown/
[2]: http://www.fileformat.info/info/unicode/char/2163/index.htm
[3]: http://www.markitdown.net/
[4]: http://daringfireball.net/projects/markdown/basics
[5]: http://daringfireball.net/projects/markdown/syntax
[6]: http://kune.fr/wp-content/uploads/2013/10/ghost-blog.jpg
