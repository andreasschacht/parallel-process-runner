# Install

Install via composer
```bash
$ composer require tonicforhealth/parallel-process-runner
```

# Usage

```php
$runner = new \Tonic\ParallelProcessRunner\ParallelProcessRunner();
$runner
    ->setMaxParallelProcess(4)
    ->add(new Process('ls'))
    ->add([
        new Process('ls'),
        new Process('ls'),
    ])
    ->run();
```

[![Code Climate](https://codeclimate.com/github/tonicforhealth/parallel-process-runner/badges/gpa.svg)](https://codeclimate.com/github/tonicforhealth/parallel-process-runner)
