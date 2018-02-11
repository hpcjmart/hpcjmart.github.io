---
title: "CloudDI: Sahara, Magnum y Manila"
layout: archive
permalink: /SeminarioCloudDI/
---

## Sahara

El proyecto Sahara nos proporciona de una manera sencilla, aprovisionar un cluster de computo intensivo, Apache Hadoop, Apache Spark y Apache Storm sobre OpenStack

El proceso de creación de un cluster se divide en cuatro fases:

* Registro de imagenes
* Creación del template de los nodos
* Creación del template del cluster
* Creación del cluster

### Registro de imágenes

Lo primero de todo, si estamos en modo linea de comandos, es decir, nos hemos conectado a la máquina de control del cluster de pruebas del Departamento de Informática a traves de ssh, es cargar las credenciales:

<pre>
hpcjmart@testcontroller:~$ source hpcjmart-rc.sh 
Please enter your OpenStack Password for project hpcjmart as user hpcjmart: 
hpcjmart@testcontroller:~$ 
</pre>

You will need to upload a virtual machine image to the OpenStack Image service. You can download pre-built images with vanilla Apache Hadoop installed, or build the images yourself. This guide uses the latest available Ubuntu upstream image, referred to as sahara-vanilla-latest-ubuntu.qcow2 and the latest version of vanilla plugin as an example. Sample images are available here:

Necesitamos ahora, cargar la imagen de la máquina virtual con el servicio de imagenes de Openstack. Podemos descargar una imagen preconfigurada con el vanilla Apache haddop instalado o bien, podemo soptar por contruir nosotros mismos las imágenes. Para este ejemplo vamos a usar la imagen [sahara-vanilla-latest-ubuntu.qcow2](http://sahara-files.mirantis.com/images/upstream/ocata/sahara-ocata-vanilla-2.7.1-ubuntu.qcow2). 

Podemos encontrar mas imagenes preconfiguradas e instaladas en la dirección [http://sahara-files.mirantis.com/images/upstream/ocata/](http://sahara-files.mirantis.com/images/upstream/ocata/)

Para poder avanzar de manera mas rápida, la imagen ya se encuentra cargada en el repositorio de OpenStack. Lo podemos ver en la opcion del menu horizon:

![Proyecto Compute Imagenes](https://hpcjmart.github.io/images/imagenes.png)


### Template de los nodos

### Template del cluster

### Creación del cluster


## Magnum

## Manila


## Blockquotes

Single line blockquote:

> Quotes are cool.

## Tables

| Entry            | Item   |                                                              |
| --------         | ------ | ------------------------------------------------------------ |
| [John Doe](#)    | 2016   | Description of the item in the list                          |
| [Jane Doe](#)    | 2019   | Description of the item in the list                          |
| [Doe Doe](#)     | 2022   | Description of the item in the list                          |

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|-----------------------------|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=============================|
| Foot1   | Foot2   | Foot3   |

## Definition Lists

Definition List Title
:   Definition list division.

Startup
:   A startup company or startup is a company or temporary organization designed to search for a repeatable and scalable business model.

#dowork
:   Coined by Rob Dyrdek and his personal body guard Christopher "Big Black" Boykins, "Do Work" works as a self motivator, to motivating your friends.

Do It Live
:   I'll let Bill O'Reilly [explain](https://www.youtube.com/watch?v=O_HyZ5aW76c "We'll Do It Live") this one.

## Unordered Lists (Nested)

  * List item one 
      * List item one 
          * List item one
          * List item two
          * List item three
          * List item four
      * List item two
      * List item three
      * List item four
  * List item two
  * List item three
  * List item four

## Ordered List (Nested)

  1. List item one 
      1. List item one 
          1. List item one
          2. List item two
          3. List item three
          4. List item four
      2. List item two
      3. List item three
      4. List item four
  2. List item two
  3. List item three
  4. List item four

## Buttons

Make any link standout more when applying the `.btn` class.

## Notices

**Watch out!** You can also add notices by appending `{: .notice}` to a paragraph.
{: .notice}

## HTML Tags

### Address Tag

<address>
  1 Infinite Loop<br /> Cupertino, CA 95014<br /> United States
</address>

### Anchor Tag (aka. Link)

This is an example of a [link](http://github.com "Github").

### Abbreviation Tag

The abbreviation CSS stands for "Cascading Style Sheets".

*[CSS]: Cascading Style Sheets

### Cite Tag

"Code is poetry." ---<cite>Automattic</cite>

### Code Tag

You will learn later on in these tests that `word-wrap: break-word;` will be your best friend.

### Strike Tag

This tag will let you <strike>strikeout text</strike>.

### Emphasize Tag

The emphasize tag should _italicize_ text.

### Insert Tag

This tag should denote <ins>inserted</ins> text.

### Keyboard Tag

This scarcely known tag emulates <kbd>keyboard text</kbd>, which is usually styled like the `<code>` tag.

### Preformatted Tag

This tag styles large blocks of code.

<pre>
.post-title {
  margin: 0 0 5px;
  font-weight: bold;
  font-size: 38px;
  line-height: 1.2;
  and here's a line of some really, really, really, really long text, just to see how the PRE tag handles it and to find out how it overflows;
}
</pre>

### Quote Tag

<q>Developers, developers, developers&#8230;</q> &#8211;Steve Ballmer

### Strong Tag

This tag shows **bold text**.

### Subscript Tag

Getting our science styling on with H<sub>2</sub>O, which should push the "2" down.

### Superscript Tag

Still sticking with science and Isaac Newton's E = MC<sup>2</sup>, which should lift the 2 up.

### Variable Tag

This allows you to denote <var>variables</var>.

{% include base_path %}
{% for post in site.pages %}
{% include archive-single.html %}
{% endfor %}
