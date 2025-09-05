## Hi there, I'm Ikbal 👋
```php
<?php

namespace MdAllamaIkbal;

/**
 * Class About
 *
 * A fun portfolio-style class that represents me as a developer.
 * You’ll get an idea of my skills, experience, and what I’m currently working on.
 *
 * @author Md Allama Ikbal
 */
class About extends Me
{
    private const UPWORK_PROFILE = 'https://www.upwork.com/freelancers/~01ae7ba3a1d21b9f1b';
    private const GITHUB_PROFILE = 'https://github.com/ikbal-559';

    public function hireMe(): string
    {
        return self::UPWORK_PROFILE;
    }

    public function getBio(): string
    {
        return <<<BIO
I am Md Allama Ikbal, a full-time freelancer with 10+ years of experience 
in backend and frontend development. I build scalable web applications 
using Laravel, Node.js, Vue.js, React.js, Next.js, Tailwind, and Bootstrap. 

I’m skilled in MySQL, PostgreSQL, MongoDB, and server management with LEMP & LAMP stacks. 
I specialize in SaaS, Hotel Management Systems, Payment Gateways, 
Real-time Applications, CMS, and CRM solutions.
BIO;
    }

    public function getExperience(): array
    {
        return [
            [
                'role' => 'Full-time Freelancer',
                'company' => 'Upwork',
                'period' => '2015 - Present',
            ],
            [
                'role' => 'Senior Backend Developer',
                'company' => 'Various Clients',
                'period' => '2012 - 2015',
            ],
        ];
    }

    public function getCurrentFocus(): array
    {
        return [
            'working_on' => [
                'Quickroom (Multi-tenant Hotel Management SaaS)',
                'Stripe & Flutterwave Payment Integrations',
                'Laravel, Inertia, Vue.js, React.js, Next.js',
            ],
            'learning' => [
                'Flutter for mobile app development',
                'Advanced system architecture & microservices',
            ],
        ];
    }

    public function getFutureGoal(): string
    {
        return 'To scale SaaS applications globally and contribute to open source.';
    }

    public function favouriteStack(): array
    {
        return ['Laravel', 'Next.js', 'Vue.js', 'Tailwind', 'MySQL'];
    }

    public function coffeeNeeded(): bool
    {
        return true; // Always true :)
    }

    public function contactMe(): array
    {
        return [
            'github' => self::GITHUB_PROFILE,
            'upwork' => self::UPWORK_PROFILE,
        ];
    }
}
