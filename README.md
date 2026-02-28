<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo" />
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<h2>Operating Systems Used</h2>

<ul>
  <li>Windows 10 (21H2)</li>
</ul>

<h2>Post-Install Configuration Objectives</h2>

<ul>
  <li>Creating Group Policies</li>
  <li>Blocking, Unblocking or change policies</li>
</ul>

<h2>Configuration Steps</h2>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/CreatedUsers.PNG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      Firstly, I've created random users using a script from internet. All these users are added
      to Domain Users group.
    </strong>
  </i>
</p>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/groupPolicies.PNG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      This is group policies and we can acces it from the administrative tools.
    </strong>
  </i>
</p>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/lockoutThreshold.PNG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      For instance here we edited computer configuration and from lockout policies we can apply
      threshold policy so that if user attempts to log in unsuccessfully more than 10 times, the
      account will be blocked.
    </strong>
  </i>
</p>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/CreatedUsers.PNG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      Firstly, I've created random users using a script from internet. All these users are added
      to Domain Users group.
    </strong>
  </i>
</p>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/blocked.JPG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      Here Iattemped to log in using wrong password more than 10 times, therefore, the account
      was blocked. In the next step I'm gonna unblock the user.
    </strong>
  </i>
</p>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/unblockAccount.PNG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      Now I'll unblock the user using Active DirectoryThe steps are following:<br />
      WIN + R -> dsa.msc -> enter -> mydomain.com -> _EMPLOYEES -> bed.rit(user's name) ->
      properties -> account -> check(Unblock the user .....) . Also we can right click on user
      and reset the password or do many other operations
    </strong>
  </i>
</p>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/lockoutThreshold.PNG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      For instance here we edited computer configuration and from lockout policies we can apply
      threshold policy so that if user attempts to log in unsuccessfully more than 10 times, the
      account will be blocked.
    </strong>
  </i>
</p>

<p>
  <img
    src="https://github.com/tabrizcyber/images/blob/main/lockoutThreshold.PNG"
    height="80%"
    width="80%"
    alt="Disk Sanitization Steps"
  />
</p>

<p>
  <i>
    <strong>
      For instance here we edited computer configuration and from lockout policies we can apply
      threshold policy so that if user attempts to log in unsuccessfully more than 10 times, the
      account will be blocked.
    </strong>
  </i>
</p>
