gojson
======

gojson attempts to generate go struct definitions from json documents


Example
----------

```sh
$ curl -s https://api.github.com/users/tmc | gojson -name=User
package main

type User struct {
	AvatarURL         string      `json:"avatar_url"`
	Bio               interface{} `json:"bio"`
	Blog              string      `json:"blog"`
	Company           string      `json:"company"`
	CreatedAt         string      `json:"created_at"`
	Email             string      `json:"email"`
	EventsURL         string      `json:"events_url"`
	Followers         float64     `json:"followers"`
	FollowersURL      string      `json:"followers_url"`
	Following         float64     `json:"following"`
	FollowingURL      string      `json:"following_url"`
	GistsURL          string      `json:"gists_url"`
	GravatarID        string      `json:"gravatar_id"`
	Hireable          bool        `json:"hireable"`
	HtmlURL           string      `json:"html_url"`
	ID                float64     `json:"id"`
	Location          string      `json:"location"`
	Login             string      `json:"login"`
	Name              string      `json:"name"`
	OrganizationsURL  string      `json:"organizations_url"`
	PublicGists       float64     `json:"public_gists"`
	PublicRepos       float64     `json:"public_repos"`
	ReceivedEventsURL string      `json:"received_events_url"`
	ReposURL          string      `json:"repos_url"`
	StarredURL        string      `json:"starred_url"`
	SubscriptionsURL  string      `json:"subscriptions_url"`
	Type              string      `json:"type"`
	UpdatedAt         string      `json:"updated_at"`
	URL               string      `json:"url"`
}
```

Installation
----------

```sh
$ go get github.com/tmc/gojson
```

License 
----------

gojson is free software distributed under Version 3 of the GNU Public License. 

As of the time of writing, this is the same license used for gcc (and therefore gccgo), so it is unlikely to restrict use in any way. Note that the GPL does not extend to any output generated by gojson; the GPL only applies to software which includes copies of gojson itself.
