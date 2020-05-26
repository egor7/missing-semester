---
layout: page
title: The Missing Semester of Your CS Education
---

Classes teach you all about advanced topics within CS, from operating systems
to machine learning, but there’s one critical subject that’s rarely covered,
and is instead left to students to figure out on their own: proficiency with
their tools. We’ll teach you how to master the command-line, use a powerful
text editor, use fancy features of version control systems, and much more!

Students spend hundreds of hours using these tools over the course of their
education (and thousands over their career), so it makes sense to make the
experience as fluid and frictionless as possible. Mastering these tools not
only enables you to spend less time on figuring out how to bend your tools to
your will, but it also lets you solve problems that would previously seem
impossibly complex.

This course functions as a module that's a jumping off point for many of the
topics in UIC's CS 361: Systems Programming: getting acquainted with
technologies like shells and docker containers are great introductions to
topics like library linking, the user/kernel boundary, and file management.

Read about the [motivation behind this class](/about/).

# Schedule

{% comment %}
**Lecture**: 35-225, 2pm--3pm<br>
**Office hours**: 32-G9 lounge, 3pm--4pm (every day, right after lecture)
{% endcomment %}

<ul>
{% assign lectures = site['f20'] | sort: 'date' %}
{% for lecture in lectures %}
    {% if lecture.phony != true %}
        <li>
        <strong>{{ lecture.date | date: '%-m/%d' }}</strong>:
        {% if lecture.ready %}
            <a href="{{ lecture.url }}">{{ lecture.title }}</a>
        {% else %}
            {{ lecture.title }} {% if lecture.noclass %}[no class]{% endif %}
        {% endif %}
        </li>
    {% endif %}
{% endfor %}
</ul>

Video recordings of the lectures are available [on
YouTube]({{site.youtube}}).

# About the class

**Staff**: This class is taught by [Chris Kanich]({{ site.ckanich }}).   
**Questions**: Email us at [{{ site.email }}](mailto:{{site.email}}).

---

<div class="small center">
<p><a href="{{ site.repository }}">Source code</a>.</p>
<p>Licensed under CC BY-NC-SA. <a href="/license/">More information about this license.</a></p>
</div>
